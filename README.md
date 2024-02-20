# Remote Shell Control

This repository contains two Python scripts for remote shell control over a network connection.

## `server.py`

This script listens for incoming connections from a target machine. It provides a command-line interface for executing commands on the target machine and transferring files between the server and the target.

### Usage

1. Run `server.py` on the machine you want to use as a control center.
2. Wait for incoming connections from the target machine.
3. Control the target machine by executing commands.

## `backdoor.py`

This script is designed to be executed on the target machine. It connects to the server and provides remote access to the target machine's shell.

### Usage

1. Modify the `connection()` function in `backdoor.py` to specify the IP address and port of the server.
2. Run `backdoor.py` on the target machine.
3. Wait for the connection to be established with the server.
4. Control the target machine remotely using the server.

## Features

- Execute shell commands on the target machine remotely.
- Upload files from the server to the target machine.
- Download files from the target machine to the server.
- Automatic reconnection functionality in case of network interruptions.

## Disclaimer

This code is provided for educational purposes only. Use it responsibly and only on systems you have permission to access.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
