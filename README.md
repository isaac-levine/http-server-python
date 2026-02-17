# HTTP Server

An HTTP/1.1 server built from scratch in Python using `asyncio`. No frameworks — just raw socket-level request parsing and response construction.

Built as a [CodeCrafters](https://codecrafters.io) challenge.

## Features

- Async request handling with `asyncio` streams
- Manual HTTP request parsing (method, path, headers, body)
- Proper HTTP response construction with status codes
- Support for `GET` and `POST` methods
- Content-Type and Content-Length header handling

## How It Works

The server:
1. Listens for TCP connections using `asyncio.start_server`
2. Reads raw bytes from the socket
3. Parses the HTTP request line, headers, and body
4. Routes the request and constructs an HTTP response
5. Writes the response bytes back to the socket

## Running

```bash
python app/main.py
```

## Built With

Python 3, `asyncio` (no external dependencies for the server itself)
