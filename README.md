# OSSP Practical Session 6

## Client–Server Application using Named Pipes (FIFOs)

### Objective

To implement a client-server application using two named pipes (FIFOs), where:

- The client sends a message to the server.
- The server receives and processes the message.
- The server sends a response back to the client.
- Multiple clients can communicate with the server.
- Each client uses a separate response FIFO.

---

## Part 1: FIFO Client-Server Application

### Files

- `fifo_server.c` – Server program
- `fifo_client.c` – Client program

### Concepts Used

- Named Pipes (FIFOs)
- `mkfifo()`
- `open()`
- `read()`
- `write()`
- `close()`
- `unlink()`
- Process IDs
- Multiple client communication

### Compilation

Compile the server:

```bash
gcc -Wall -Wextra -o fifo_server fifo_server.c
