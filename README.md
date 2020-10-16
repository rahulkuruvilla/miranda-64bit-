# Guide to installing a 64-bit version of Miranda on your machine #

I couldn't find a guide detailed enough online installing Miranda on a 64-bit only compatible Mac so I made one myself. 
Note: the version online is the source which needs to be compiled before execution.
The repo contains the details to install miranda v2.066 from source or a compiled 64-bit version contained in this repo.

## Installing from source ##

Run `sh mira_compile.sh` in this repo.

Alternatively, run the following commands from the `miranda` folder:
```bash
make cleanup
make 
sudo make install
```

## Installing the binary ## 

Run :

```bash
sudo tar xzpf mira.tgz -C /
```

Installs the binary to the /usr/local dir, rather than /usr dir. Refer to the makefile for further detail. This workaround is to eliminate the need to disable SIP protection on a Mac.

## Running miranda ## 

To run miranda just run the terminal command: 
```bash
mira
```

