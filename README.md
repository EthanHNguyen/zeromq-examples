# Python ZeroMQ Example

This repository contains an example of ZeroMQ messaging using the Request-Reply pattern. It consists of four sockets: a REQ socket, two ROUTER sockets, and a DEALER socket. The message flow is as follows:

    REQ -> ROUTER1 -> DEALER -> ROUTER2 -> REQ (replies)

At each step, the message is printed to the console.

## Installation

To run this example, you will need to have Python 3 and ZeroMQ installed. A conda environment.yaml is provided.

## Usage

Once you have created the conda environment and installed PyZMQ, you can run the example by running the following command:

```
conda activate zmq
python req_router_dealer_router.py
```

## License

This example is licensed under the MIT License.

