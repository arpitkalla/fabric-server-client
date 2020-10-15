# Server Client communication using LibFabric

## Setup
Requires `libfabric`, on OSX `brew install libfabric`
Run `make` to compile.
### Server
Run `./main -s`, this would start the server on port `9000`

1. Accept mutiple connections
2. Have a thread to read data in memory

### Client
Run `./main <SERVER_IP> <NUM_THREADS> <SIZE> <COUNT>` to run the client.
1. Create a connection to the server
2. Send bytes using RDMA


## TODO
- [ ] Create Golang wrapper for C++ code
- [ ] Find a way to calcuate latency
