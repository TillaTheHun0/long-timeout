# Long timeouts

Long timeout makes it possible to have a timeout or interval that is longer than 24.8 days (2^31-1 milliseconds).


## Usage

```js
var lt = require('long-timeout')

var timeout = lt.setTimeout(function() {
  console.log('in 30 days')
}, 1000 * 60 * 60 * 24 * 30)


// Clear it
lt.clearTimeout(timeout)
```

```js
var lt = require('longtimeout')

var interval = lt.setInterval(function() {
  console.log('every 30 days')
}, 1000 * 60 * 60 * 24 * 30)

// Clear it
lt.clearInterval(interval)
```

## Install

    npm install long-timeout


## Licence

MIT
