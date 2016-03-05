# GlaDus

*GlaDus* is a personal home automation system running on a Raspberry Pi Model B+ and built on top of the open source Openhab framework.


## Architecture

#### Devices

* Raspberry Pi Model B+
* Tellstick Duo
    + Switches
    + Dimmer
    + Remote
* Temperature / humidity sensor

#### Bindings

- Tellstick
- HTTP
- rrd4j

## Configuration

See https://github.com/openhab/openhab/wiki/Quick-Setup-an-openHAB-Server for Openhab's setup instructions. Below is a short summary of my personal configs.

#### Items

- Lights
- Remote switches
- Temperature
- Humidity
- Volume

#### Rules

- Volume control
- Remote control for lights
    + Regular remote switch
    + A timer that turns a light on for a 1 minute before automatically turning off (good for saving effort and energy)

#### Persistence

-rrd4j persistence
    - Every minute: Temperature and humidity
    - Every change: Lights

#### Sitemaps





