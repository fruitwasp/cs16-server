Docker file for a Counterstrike 1.6 server with some custom settings (see server.cfg).


```bash
git clone git@github.com:jorisvandesande/cs16-server.git
cd cs16-server
docker build .
```

Use the hash that will be emitted by the `docker build` command as `<image_name>` when starting the container:
```bash
docker run -p 26900:26900/udp -p 27020:27020/udp -p 27015:27015/udp -p 27015:27015 -d <image_name>
```
