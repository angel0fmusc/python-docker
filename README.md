# python-docker
A Python script to look up company names from a given MAC address. Dockerfile included to create a Docker image to run the script as an executable. Both the script and image will expect a commandline argument when the script/ container is run.

### Security
Anyone is able to utilize the script obtain a company name given any MAC address. If security was to be integrated, only certain users could access or use the script.

## Installation
Linux (script only):

```
$ pip install requests
```

Dockerfile build:
- Docker Engine already installed
- Dockerfile and script must be in the same directory
```
$ docker build -t [YOUR IMAGE NAME] .
```


## Usage
The script expects a command line argument of a MAC address
```
$ python MAC_Addr_Lookup.py [MAC Address]
```

Docker
```
$ docker run [YOUR IMAGE NAME] [MAC Address]
```


## API
- [macaddress.io](https://macaddress.io/api) - Retrieve vendor information given the MAC Address or OUI

## Related
- [Docker CE](https://docs.docker.com/v17.12/install/linux/docker-ce/ubuntu/) - Documentation to install Docker CE on Ubuntu
