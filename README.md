# XCarve Proxy
A Node.js proxy server for connecting to a remote XCarve via a Raspberry Pi that is running [xcarve-server][1].

## Installation

Make sure you have the latest stable version of [Node.js][3] installed on your computer.

```
$ node -v
v0.12.6
```
Install `forever` and `xcarve-proxy` on your computer using `npm`.

```
$ npm install -g forever xcarve-proxy
```

## Starting the Daemon
Make sure you have [xcarve-server][1] running on your Raspberry Pi before continuing. If everything has
been setup properly, you can start the proxy daemon by running the following command:

```
$ xcarve-proxy

██╗  ██╗      ██████╗ █████╗ ██████╗ ██╗   ██╗███████╗
╚██╗██╔╝     ██╔════╝██╔══██╗██╔══██╗██║   ██║██╔════╝
 ╚███╔╝█████╗██║     ███████║██████╔╝██║   ██║█████╗
 ██╔██╗╚════╝██║     ██╔══██║██╔══██╗╚██╗ ██╔╝██╔══╝
██╔╝ ██╗     ╚██████╗██║  ██║██║  ██║ ╚████╔╝ ███████╗
╚═╝  ╚═╝      ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝  ╚═══╝  ╚══════╝

starting proxy daemon on port 1338...
```

Visit [easel.inventables.com][2] to test out the proxy.

## Stopping the Daemon

```
$ forever stopall
```

[1]: https://github.com/adafruit/xcarve-server
[2]: http://easel.inventables.com
[3]: https://nodejs.org
