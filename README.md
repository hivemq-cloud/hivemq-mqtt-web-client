hivemq-mqtt-web-client
======================

## Cloud Deployment

This repo is a fork of the open source client in the `hivemq` organisation. It was forked to ensure that no open source contributions get deployed to the websocket client we're linking to in the customer facing frontend (currently named Portal) without approval by the cloud team.

A [Github Action](https://github.com/hivemq-cloud/hivemq-mqtt-web-client/actions/workflows/repo-sync.yaml) is syncing the changes from the open source master branch to the destination branch `upstream` of this fork.

The client used for Cloud is deployed via [Netlify](https://github.com/hivemq-cloud/hivemq-mqtt-web-client/actions/workflows/repo-sync.yaml). 

*IMPORTANT*: All changes to the master branch of this repository will be available in production immediately!
## A websockets based MQTT Client for your browser.

This client runs on any modern browser, which supports websockets (sorry Internet Explorer <10!).
You can use it to publish and subscribe at the same time.

See it in action at [http://hivemq.com/demos/websocket-client/](http://www.hivemq.com/demos/websocket-client/ "MQTT Websocket Client")

## How to use it

Read the blog post about ["A full-featured MQTT client for your browser"](http://www.hivemq.com/full-featured-mqtt-client-browser/ "A full-featured MQTT client for your browser")


## Localhost / Local network

You can also use this client to connect to a broker on your local machine ("localhost") or any machine in your local network which is reachable from the machine which your browser runs on.



## MQTT Broker

This web client works perfectly with the [HiveMQ MQTT broker](https://www.hivemq.com/hivemq/ "HiveMQ MQTT Broker") with enabled websockets.

If you don’t like to use a self hosted (or locally running) HiveMQ, you can use the [public MQTT broker](http://www.hivemq.com/showcase/public-mqtt-broker/ "Public MQTT Server") from the [MQTTDashboard](http://www.mqttdashboard.com/ "MQTT Dashboard").

* Host: **broker.mqttdashboard.com**
* Websockets port: **8000**


## Why another MQTT Client

We at [HiveMQ](https://www.hivemq.com/ "HiveMQ") needed a quick and simple way to develop and test our applications which use MQTT over websockets, so we sat down for a few hours and built this client which also works for your local development machine.

## Can I embedd it / ship it with my software?

Sure! We would however be very glad if you would honor the work by linking to the original client source or mentioning that this websocket client was developed initially for HiveMQs websocket support. 

# Contributing

If you want to contribute to HiveMQ MQTT Web Client, see the [contribution guidelines](CONTRIBUTING.md).

# License

HiveMQ MQTT Web Client is licensed under the `APACHE LICENSE, VERSION 2.0`. A copy of the license can be found [here](LICENSE).

