# Moisture_Reporter
This is ESP8266 code to measure the moisture in the ground with a capacitive moisture probe and report it via MQTT.

 Configuration is done via serial connection.  Enter:
  *  broker={broker name or address}
  *  port={port number}   (defaults to 1883)
  *  topicroot={topic root} (something like buteomont/water/pressure/ - must end with / and 
  *  "percent" or "value" will be added)
  *  user={mqtt user}
  *  pass={mqtt password}
  *  ssid={wifi ssid}
  *  wifipass={wifi password}
  *  wet={reading when sensor in saturated soil}
  *  dry={reading when sensor is in dry soil}
  *  sleepTime={seconds to sleep between measurements} (set to zero for continuous readings)
  *  debug={1|0} to turn serial port debug statements on or off`
 
 Some configuration parameters can be set via MQTT topic $TOPICROOT/command.
