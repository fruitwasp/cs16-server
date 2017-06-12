Docker file for a Counterstrike 1.6 server with some custom settings (see server.cfg).


```bash
docker pull jorisvandesande/cs16-server
```

Then start the container with the following command to expose the server to your network:
```bash
docker run -p 26900:26900/udp -p 27020:27020/udp -p 27015:27015/udp -p 27015:27015 -d jorisvandesande/cs16-server
```
