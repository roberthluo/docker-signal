# docker-signal
Container for running signal-desktop

## Build with
docker build -t signal signal

## Run with
docker run --rm -d -v /tmp/.X11-unix/:/tmp/.X11-unix -v $HOME/container-home:/root -e DISPLAY -e XAUTHORITY -v $XAUTHORITY:$XAUTHORITY --net=host signal

You will need a directory called 'container-home' in your home directory
for storing state.
