# Phillip's Hue Zetta Driver

[Zetta](http://zettajs.io) device package for Phillips Hue Driver, use this to discover Hue hubs and bulbs on your [Zetta](http://zettajs.io) platform. Uses the [Node Hue Api](https://github.com/peter-murray/node-hue-api) from Peter Murray to communicate with Hue hub and bulbs.

## Install

```
npm install zetta-hue-driver
```

## Usage

```js
var zetta = require('zetta');
var Hue = require('zetta-hue-driver');

zetta()
  .use(Hue)
  .listen(1337);
```

## Register your hub

As a security measure, you must register your hub in order for the `zetta-hue-driver` to find your connected bulbs. 

To do this: 
  1. push the `link` button on top of your hue hub 
    * the same physical button you pushed when you linked your hub to your mobile app or web account 
  2. trigger the `regiser` action in the zetta api. 
    * You'll have 10-20 seconds to do this before the api times out.   

## License

MIT
