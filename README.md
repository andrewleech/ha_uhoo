# uHoo air quality monitor custom component for Home Assistant

A air quality monitoring appliance, which syncs data to the cloud.

This API seems to only be available for enterprise customers currently but speak to uHoo if you have questions about that. Alpha quality but again, low risk, as it's only pulling data...should move towards beta quality quickly. Built on top of [pyuhooair](https://github.com/netmanchris/pyuhooair).

* Support for CO, CO<sub>2</sub>, NO<sub>2</sub>, O<sub>3</sub>, TVOC, Dust(PM2.5), Humidity and Air Pressure.
* No support for Temperature yet, as there is a bug in the underlying python module.
* Only updates from the API every 15 mins, data is cached by the pyuhooair implementation.

Configuration just needs email address and password:

```YAML
sensor:
  - platform: uhooair
    email: user@email.com
    password: SuperSecret12345
```
