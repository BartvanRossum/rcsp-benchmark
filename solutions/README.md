# Solution File Format

Each solution file `solution_s{S}_t{T}.txt` contains one duty per line.
Each line is a space-separated list of connection indices, corresponding to a valid duty in the instance `s{S}_t{T}`.

A duty is a path SOURCE → CONNECTION* → SINK in the connection graph defined by `connections.txt`.
The connection indices refer to the `index` field in `connections.txt`.

These are the best known solutions found throughout the experiments in the accompanying paper.
