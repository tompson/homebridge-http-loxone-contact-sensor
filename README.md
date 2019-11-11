# homebridge-http-loxone-contact-sensor

This is a plugin for [homebridge](https://github.com/nfarina/homebridge) which can monitor Contact / Door sensor via a HTTP endpoint of the Loxone web services.

## Install

Previous installation of [Homebridge](https://github.com/nfarina/homebridge) is required.

Then run the following command to install `homebridge-http-loxone-contact-sensor`

```
npm install -g homebridge-http-loxone-contact-sensor
```

## Configuration

```json
{
    "accessory": "LoxoneContactSensor",
    "name": "Front Door",
    "pollInterval": 1000,
    "statusUrl": "http://miniserver/jdev/sps/io/WindowName/state"
}
```

> You can add as many accessories as needed.

**Example homebridge configuration**


```json
{
    ...
    "accessories": [
        {
            "accessory": "LoxoneContactSensor",
            "name": "Front Door",
            "pollInterval": 500,
            "statusUrl": "http://miniserver/jdev/sps/io/WindowName/state"
        }
    ],
    "platforms": [
        ...
    ]
}
```
