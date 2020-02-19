
# Node Demonstration

This demo allows you to see different components of the Node software working together, processing incoming events.

Follow the guide to run it with docker-compose and observe the printout.

## Node Demonstration Guide

#### If you don't have Docker Compose
If you don't have Docker Compose, please follow [official installation guide](https://docs.docker.com/compose/).

#### Run with Docker Compose
Clone this repository, and execute `docker-compose up`, it will start the client and the server, after downloading and building docker images (only on the first run).

The server is one of the nodes, that listens for events. The client sends random events to a server.

#### What Happens Behind The Scenes
Node communicates those events to other nodes, and all of them build a Hashgraph. Ones the Hashgraph Round is decided, meaning all nodes have the same graph up until one defined point, the events are sorted and executed.
