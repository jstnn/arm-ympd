# arm-ympd

This is an image for the MPD Web GUI [ympd](https://www.ympd.org/) using Debian. A [Resin.os Raspbian image](https://hub.docker.com/r/resin/rpi-raspbian/) is used as a base image for compatibility with IoT devices, but it works well anywhere. This is an add-on for MPD.

# How to use 

    docker run -p 8080:8080 --name=ympd -d jstnn/arm-ympd:latest

An instance of icecast is now running with the port 8080 mapped to your host or docker-machine IP address.

# Custom configuration 

You can edit the information in the frontend, using your browser.

# Credits

This dockerfile is based on the [alpine-ympd image](https://hub.docker.com/r/vitiman/alpine-ympd/). Changes has been made to compile with an IoT device with an ARMv7 architecture like the RaspberryPi 3 using a resin.os optimized image.
