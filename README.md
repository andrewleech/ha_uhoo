# uHoo air quality monitor custom component for Home Assistant

A air quality monitoring appliance, which syncs data to the cloud.

Built on top of [pyuhoo](https://github.com/netmanchris/pyuhoo), this module is intended to work with the consumer api for uHoo. No guarantees are given that it will continue to work however.

* Support for Temperature, CO, CO<sub>2</sub>, NO<sub>2</sub>, O<sub>3</sub>, TVOC, Dust(PM2.5), Humidity and Air Pressure.

Configuration just needs email address and password:

```YAML
sensor:
  - platform: uhooair
    email: user@email.com
    password: SuperSecret12345
```
