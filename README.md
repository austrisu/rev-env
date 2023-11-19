# Docker Codespace for Reverse CTF
This Docker Codespace is designed for use in reverse CTF (Capture The Flag) challenges. It provides a pre-configured environment with various tools commonly used in reverse engineering tasks. The Docker image is based on Ubuntu 20.04 and includes the following tools:

### Development Tools:

- Git
- Clang-format
- Ninja-build
- GDB (GNU Debugger)
- Python 3 and essential development packages
- Strace
- Vim, Nano, Less

### Binary Analysis Tools:
- Binwalk
- File
- Binutils
- Ropper

### Debugging Tools:
- Pwngdb (GDB plugin for exploit development)
- Radare2 (Reverse engineering framework)

### Static Analysis Tools:
- Miasm (Reverse engineering framework)
- Frida (Dynamic instrumentation toolkit)
- Lief (Library to Instrument Executable Formats)
- Pefile (Python module to read and work with PE files)

### Binary Exploitation Tools:
- Angr (Binary analysis framework)
- Xortool (Tool for analyzing multi-byte XOR ciphers)

### Additional Tools:
- Oh My Bash (A delightful community-driven framework for managing your bash configurations)

## Usage
To use this Docker Codespace, follow these steps:

Build the Docker image using the provided Dockerfile.
```bash
docker build -t reverse-ctf .
```

Run the Docker container based on the built image.
```bash
docker run -it reverse-ctf
```

You will now have a fully configured environment with all the necessary tools for reverse CTF challenges.
Feel free to customize the Dockerfile further to suit your specific needs or to include additional tools as required for your reverse CTF scenarios. Happy reversing!
