_Component to integrate with uHoo._

uHoo is an air quality monitor which syncs data to the cloud.

Built on top of [pyuhoo](https://github.com/netmanchris/pyuhoo), this module is intended to work with the consumer api for uHoo. No guarantees are given that it will continue to work however.

* Support for Temperature, CO, CO<sub>2</sub>, NO<sub>2</sub>, O<sub>3</sub>, TVOC, Dust(PM2.5), Humidity and Air Pressure.

**This component will set up the following platforms.**

Platform | Description
-- | --

_TBD_
<!---
`binary_sensor` | Show something `True` or `False`.
`sensor` | Show info from blueprint API.
`switch` | Switch something `True` or `False`.
-->

{% if not installed %}
## Installation

1. Click install.
2. Add the following to configuration.yaml
```YAML
sensor:
  - platform: uhooair
    email: user@email.com
    password: SuperSecret12345
```
{% endif %}
