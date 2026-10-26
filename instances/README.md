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

## connections_single_depot.txt / connections_multi_depot.txt

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

A valid duty is a path SOURCE → CONNECTION* → SINK in the connection graph, where the SOURCE and SINK connections use the same depot station.

`connections_single_depot.txt` only has SOURCE/SINK connections to/from the single station in `crewbases_single_depot.txt`. `connections_multi_depot.txt` additionally has SOURCE/SINK connections for every other station, so a duty may use any station as its depot (see `crewbases_multi_depot.txt`). Every connection in `connections_single_depot.txt` has the same index and fields in `connections_multi_depot.txt`, so a feasible single-depot solution is also a feasible multi-depot solution.

---

## stations.txt

One station per line. Fields (space-separated):

```
index  name
```

All large stations in the infrastructure network, which are the candidate start and end points for tasks. The number of large stations equals `S` in the instance name.

---

## crewbases_single_depot.txt / crewbases_multi_depot.txt

Same format as `stations.txt`. `crewbases_single_depot.txt` lists the single station that serves as the crew base (depot) in the single-depot variant. `crewbases_multi_depot.txt` lists every station in `stations.txt`, since any of them may serve as a crew base in the multi-depot variant.

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
