# GoLServer

### Overview

GoLServer contains the engine for the Game of Life simulation. It contains the following:
* Stubs - contains the structs and function names for client-server RPC calls
* Server - deals with client interaction
* Distributor - delegates work to the workers
* Worker - processes its allocated strip of the Game of Life

See `report.pdf` for more information on the project. See my GoLClient repository for the client-side controller code. See my GoLParallel repository for an alternative parallel version of the simulation.

### How to run

To run the Game of Life simulation, complete the following steps:

1. Start the server using the command `go run .` while in the GoLServer directory
1. Start the client using the same command while in the GoLClient directory
1. Use keypresses to control behaviour of the client:

's' = save current world 
| 'p' = pause/resume the simulation
| 'q' = quit the client without killing the server
| 'k' = kill the server and quit the client
