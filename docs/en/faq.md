![Logo](../../admin/shelly.png)

# ioBroker.shelly

## Can I use CoAP and MQTT at the same time?

No, but you can create a second instance of the Shelly adapter which is configured with MQTT (and the other one with CoAP).

## I don't know anything about MQTT, is it hard to use?

No, just configure your shelly devices as documented [here](protocol-mqtt.md) and the Shelly adapter will handle everything else.

## Can I switch between CoAP and MQTT? What will happen?

You can re-configure your instance at any time. You will not loose any objects or states and everything will stay the same. Just the communication method changes changes in the background.

## Is it possible to connect the Shelly adapter to an existing MQTT broker?

It is not possible to connect the Shelly adapter to an existing MQTT broker in your network. The Shelly adapter starts an own broker which is running on the (non default) port ``1882`` to avoid conflicts with other MQTT brokers on the same system.