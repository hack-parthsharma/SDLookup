sdlookup 
==========
IP Lookups for Open Ports and Vulnerabilities from [internetdb.shodan.io](https://internetdb.shodan.io/)

This is a golang version of [nrich](https://gitlab.com/shodan-public/nrich) which support concurrency and more efficient output.

## Install

```shell
go install github.com/hack-parthsharma/SDLookup@latest
```

## Usage

```shell
# Basic Usage
echo '1.2.3.4' | sdlookup -open
1.2.3.4:80
1.2.3.4:443

# lookup CIDR range
echo '1.2.3.4/24' | sdlookup -open -c 20
1.2.3.4:80
1.2.3.5:80

# get raw JSON response
echo '1.2.3.4' | sdlookup -json

```

