# Route Planning Project 

This is the Route Planning project for "C++ Engineer" Nanodegree at Udacity.

## Compiling and Running

### Compiling
To compile the project, first, create a `build` directory and change to that directory:
```
mkdir build && cd build
```
From within the `build` directory, then run `cmake` and `make` as follows:
```
cmake ..
make
```
### Running
The executables will be placed in the `bin` directory. From within `build`, you can run the project as follows:
```
../bin/<name-of-parent-directory> -f ../map.osm
```
A map.osm is included. However, you can give your own map file.
Once the executable file is run, the program will ask for a Start and Finish point coordinates.
Then the map is visualized with the shortest path from the Start to the Finish point. 

## Testing

For functions that have unit tests, the project must be built with the approprate test cpp file. This can be done by passing a string with the `-DTESTING` flag in `cmake`. For example, from the build directory:
```
cmake -DTESTING="RouteModel" ..
make
```
Those commands will build the code with the tests for the "Fill Out Route Model" part. The tests can then be run from the `build` directory as follows:
```
../bin/test
```
Chunks with tests will specify which string to pass with `-DTESTING`, but a table is given below with the complete list for reference:

| Exercise Name               | `-DTESTING` String Value |
|-----------------------------|:------------------------:|
| Fill Out Route Model        |       "RouteModel"       |
| Fill Out Node Class         |       "RMNodeClass"      |
| Create RouteModel Nodes     |        "RMSNodes"        |
| Write the Distance Function |        "NodeDist"        |
| Create Road to Node Hashmap |       "NodeToRoad"       |
| Write FindNeighbors         |      "FindNeighbors"     |
| Find the Closest Node       |       "FindClosest"      |
| Write the A\* Search Stub   |        "AStarStub"       |
| Finish A\* Search           |       "AStarSearch"      |

