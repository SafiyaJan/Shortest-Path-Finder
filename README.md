# Shortest-Path-Finder
In graph theory, the shortest path problem consists of finding a path between 2 vertices in a given graph such that the path is shortest among all possible paths between the 2 vertices. Finding the shortest between vertices has several applications in the real world including finding the short path between 2 physical location - just like what Google Maps does. The program in this repository, written in C++, takes as input, an edge-list of a graph and the 2 vertices, where the shortest path between the 2 vertices is to be found. In order to calculate the shortest path, the Breadth First Algorithm has been used.

## Getting Started

In order to run the program, firstly, you must clone the repository on your local machine. You can do this by running the following line on your machine's CLI:

```git clone https://github.com/SafiyaJan/Shortest-Path-Finder.git```

### Prerequisites

- Ensure that you have the latest version of CMake installed on your local machine. You can checkout the following link to download CMake for your specific machine: https://cmake.org/download/
- You will also need a C++ compiler in order to compile the program. GCC and Clang are 2 such compilers and either can be used to compile the program
  - Installing Clang - https://clang.llvm.org/get_started.html
  - Installing GCC - https://gcc.gnu.org/wiki/InstallingGCC

## Usage 

### Building the Executable

Before, the program can be run, it first needs to be built (aka compiled). Run the following command to build the program on you CLI:
```
mkdir build && cd build && cmake ../ && make 
``` 
The build sequence, creates the ```shortest_path``` executable in the ```/build``` that can now be run!

#### Running the Program
To run the executable, type the following command on your CLI:
```./shortest_path```

#### Usage Example - Finding the shortest path 
To find the shortest path on a given graph, first enter the number of vertices in the graph, the edge-list of the graph, along with the 2 verticies who's shortest path is to be found. Following is an example:

```
# Input Format must be as follows:
V <Number of Vertices in Graph>
E {<Vi,Vj>,...} # where Vi and Vj are vertices in the graph

# Example usage
V 15  
E {<2,6>,<2,8>,<2,5>,<6,5>,<5,8>,<6,10>,<10,8>} # edges in graph
s 2 10

# output from program
2-6-10  # shortest path between 2 and 10
```
