_Component to integrate with uHoo._

uHoo is an air quality monitor which syncs data to the cloud.

The API seems to only be available for enterprise customers currently but speak to uHoo if you have questions about that. Alpha quality but again, low risk, as it's only pulling data... should move towards beta quality quickly. Built on top of [pyuhooair](https://github.com/netmanchris/pyuhooair).

* Support for CO, CO<sub>2</sub>, NO<sub>2</sub>, O<sub>3</sub>, TVOC, dust (PM2.5), humidity and air pressure
* No support for temperature yet, as there is a bug in the underlying Python module
* Only updates from the API every 15 mins. Data is cached by the pyuhooair implementation

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
