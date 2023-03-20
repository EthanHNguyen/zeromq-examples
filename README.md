# Python ZeroMQ Example

This repository contains an example of ZeroMQ messaging using the Request-Reply pattern. It consists of four sockets: a REQ socket, two ROUTER sockets, and a DEALER socket. The message flow is as follows:

    REQ -> ROUTER1 -> DEALER -> ROUTER2 -> REQ (replies)

At each step, the message is printed to the console.

## Installation

To run this example, you will need to have Python 3 and ZeroMQ installed.

### Conda

If you do not have conda installed, you can download and install it from [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).

Once conda is installed, you can create a new environment with the necessary dependencies using the following command:

```
conda create --name pyzmq python=3 zmq
```

This will create a new conda environment called `pyzmq` with Python 3 and ZeroMQ installed.

### PyZMQ

To install PyZMQ,

```
conda install pyzmq
```

## Usage

Once you have created the conda environment and installed PyZMQ, you can run the example by running the following command:

```
conda activate zmq
python req_router_dealer_router.py
```

## License

This example is licensed under the MIT License.

