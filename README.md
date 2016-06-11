# Fastest-DNS

Arranges DNS Servers in /etc/resolv.conf according to the fastest

### What is it?
  Fastest-DNS is a Linux package written in Python, which checks DNS servers in /etc/resolv.conf, check for the fastest and arrange them by their speed. 
  Making fastest one the primary server for faster nameserver resolving

### Installation 
To install, just clone this repository or download
```sh
$ git clone https://github.com/donjajo/fastestDNS.git
```

### Dependencies
* dig
* Python 3.5 and above 

### Documentation
After installing, run:
```sh
$ sudo ./fastest-dns
```
This checks for DNS servers in /etc/resolv.conf and set them according to their response speed

Ignore local DNS server if present in /etc/resolv.conf
```sh
$ sudo ./fastest-dns -i
```
Provide a custom domain name to test servers with (default is google.com)
```sh
$ sudo ./fastest-dns -d facebook.com 
```
