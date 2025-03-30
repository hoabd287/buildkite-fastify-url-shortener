# URL Shortener

A URL Shortener Application built with Node.js, Fastify and PostgreSQL. See the
[final branch](https://github.com/betterstack-community/node-url-shortener/tree/final)
for the updated code with Docker configuration.

**Tutorial**:
[A Comprehensive Guide to Dockerizing Node.js Applications](https://betterstack.com/community/guides/scaling-nodejs/dockerize-nodejs/)

![URL Shortener Application](screenshot.png)

## 🟢 Prerequisites

- Prior Node.js development experience.
- Familiarity with the Linux command-line.
- Access to a Linux machine with
  [Docker Engine](https://docs.docker.com/engine/install/) installed.

## Getting started

Find the set up instructions in
[step 1 of the article](https://betterstack.com/community/guides/scaling-nodejs/dockerize-nodejs/#step-1-setting-up-the-demo-project).

## How to use

- Enter a URL into the input field and click **Shorten!**. The shortened URL
  will be displayed on the page.
- Click the **Visit** button to open the shortened URL in a new tab. It should
  redirect you to the original URL.


## Docker on Windows
Docker desktop is running under WSL system, so all the container will use WSL's IP to talk to local machine.
To look up for WSL's IP:
```
  ╱  ╱  ~ ​ ipconfig

Windows IP Configuration
Ethernet adapter vEthernet (WSL):

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::7827:62c2:e593:e8b1%47
   IPv4 Address. . . . . . . . . . . : 172.29.128.1
   Subnet Mask . . . . . . . . . . . : 255.255.240.0
   Default Gateway . . . . . . . . . :
```
- Also you should use hostname for the talk between containers.
- set github fine-grained token permission to allow access `content`
- add buildkite's webhook to github
- run first pipeline