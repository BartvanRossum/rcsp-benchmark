# Instance File Format

Each instance folder `s{S}_t{T}` contains the following files.

---

## tasks.txt

One task per line. Fields (space-separated):

```
index startTime  endTime  startStation  endStation  duration
```

- `index` — unique task identifier
- `startTime`, `endTime` — start and end time in seconds from midnight
- `startStation`, `endStation` — indices of the start and end station (see `stations.txt`)
- `duration` — task duration in seconds (`endTime - startTime`)

---

## connections.txt

One connection per line. Fields (space-separated):

```
index  type  startBlock  endBlock  timeBeforeBreak  timeAfterBreak  duration  cost
```

- `index` — unique connection identifier
- `type` — `SOURCE` (depot to first task), `SINK` (last task to depot), or `CONNECTION` (between two tasks)
- `startBlock` — for SOURCE: station index of the depot; for others: index of the preceding task
- `endBlock` — for SINK: station index of the depot; for others: index of the following task
- `timeBeforeBreak`, `timeAfterBreak` — time in seconds before and after a meal break; `-1` if no break on this connection
- `duration` — connection duration in seconds
- `cost` — connection cost in units (variable cost of 1 unit/second, plus a fixed cost of 28,800 units on SOURCE connections)

A valid duty is a path SOURCE → CONNECTION* → SINK in the connection graph.

---

## stations.txt

One station per line. Fields (space-separated):

```
index  name
```

All large stations in the infrastructure network, which are the candidate start and end points for tasks.

---

## crewBases.txt

Same format as `stations.txt`. Lists the subset of stations that serve as crew bases (depots). The number of crew bases equals `S` in the instance name.

---

## tracks.txt

One track per line. Fields (space-separated):

```
fromStation  toStation  duration
```

- `fromStation`, `toStation` — station indices
- `duration` — travel time in minutes

Describes the bidirectional infrastructure network used to generate the instance. Provided for reference and visualisation; not required by the solver.

---

## geoStations.txt

One station per line. Fields (space-separated):

```
index  name  x  y  population  isLarge
```

- `x`, `y` — coordinates on the generation grid (arbitrary units)
- `population` — synthetic population value used during demand generation
- `isLarge` — `true` for large stations (crew base candidates), `false` for small stations

Provided for reference and visualisation; not required by the solver.
