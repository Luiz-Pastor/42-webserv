# 42cursus_webserv

Webserv is a lightweight HTTP/1.1 server written in C++ that supports essential web functionalities, including: Handling GET, POST, and DELETE requests, cookies management, CGIs (Common Gateway Interface) execution and custom configurations via configuration file. It supports the following features:
- **Multi-client** support using non-blocking I/O
- **Static file serving** (HTML, CSS, JS, images, etc.)
- Dynamic content execution via **CGI** scripts
- **Request** parsing and **response** generation
- Error handling with **custom error pages**
- Basic session management via **cookies**
- **Custom configuration** for defining virtual hosts, ports, and CGI settings

To see a list of all the possible configurations supported by the project, check out the [WIKI](https://github.com/Luiz-Pastor/webserv/wiki/Configuration-File-and-Supported-Directives).

![LINUX](https://img.shields.io/badge/Linux-a?style=for-the-badge&logo=linux&color=grey)
![Docker](https://img.shields.io/badge/Docker-20232A?style=for-the-badge&logo=docker&color=b7e6ff)
![C++](https://img.shields.io/badge/C++-a?style=for-the-badge&logo=C%2B%2B&color=purple)
![Makefile](https://img.shields.io/badge/Makefile-a?style=for-the-badge&logo=monster&logoColor=orange&color=ffc56f)

You can see the subject in the intra page

## Installing and running the project:

1- Clone this repository
	
	git clone https://github.com/Luiz-Pastor/webserv.git
2- Navigate to the new directory and run `make`
	
	cd webserv
   	make
3- Start the server, a config file is needed as an argument:

	./webserv path/to/config_file

## Compiling the Program
Webserv comes with a Makefile that includes the following rules:

- `all`: compiles the program.
- `re`: recompiles the program.
- `clean`: removes obj directory with objects files.
- `fclean`: removes obj directory with objects files and webserv binary.
- `r or run`: compiles the program and launchs it with a default configuration file.
- `v or valgrind`: compiles the program and launchs it with a default configuration file using Valgrind.
- `nd or no_debug`: compiles the program and launchs it without debug prints.
- `siege`: compiles the program, launchs it and use siege to stress test the server.
