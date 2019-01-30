# clbarc-iot-protocols

## Workshop Guide for IoT Protocols

### Websockets

In your browser open the following url `http://www.hivemq.com/demos/websocket-client/`

Use `broker.hivemq.com` for our host for Websockets

### MQTT from the CLI

Open a Terminal window using iTerm or basic mac Terminal.

First we will subscribe to specific topic that we will test on.

`mosquitto_sub -h broker.hivemq.com -p 1883 -t devnetzone/topic`

`mosquitto_pub -h broker.hivemq.com -p 1883 -t devnetzone/topic -m "hello world"`

`mosquitto_sub -h broker.hivemq.com -p 1883 -t "devnet/city/#"`

### MQTT using UI

Open MQTT FX on your Mac computer.

### Python MQTT examples
Create a directory for us to work in.

`$ mkdir iot-prot`

`$ cd iot-prot`

Now let's clone the code we will need in this workshop.

`$ git clone https://github.com/JockDaRock/iot-protocols`

Change directories into the our Python code base

`cd ./iot-protocols/mqtt`

But first we need to install a python library to run our code samples.

`pip3 install paho-mqtt`

Next we will run our python program.

`python3 mqtt_sub.py`

Now, we need to open a separate terminal from where our **mqtt_sub.py** file is running.

And then we will run the python publisher application.

`python3 mqtt_sub.py`

You did it!  You are now and expert in IoT protocols ;)!





