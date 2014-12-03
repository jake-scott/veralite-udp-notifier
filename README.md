veralite-udp-notifier
=====================

Veralite Z-Wave UDP notifier

This LUA plugin for the Veralite Z-Wave controller binds to all switch,
dimmer and scene controllers, and to security sensors like the Fibaro
Universal Binary Sensor.  It sends data to the network as a broadcast
UDP packet, with the following format :
  ZWave:<type>:<id>:<name>:<value>

  .. where :
    type:   One of [Switch, Scene, Dimmer, SecuritySensor]
    id:     The index of the device, assigned at pairing time
    name:   Name of the device, assigned through the Veralite GUI
    value:  Value, specific to the device type


