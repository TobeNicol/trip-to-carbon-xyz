trip-to-carbon
==============

A wrapper for the [Trip to Carbon API](https://triptocarbon.xyz/).

Usage:

```javascript
import { carbonFootprint } from '../trip-to-carbon'

const taxiFootprint = await carbonFootprint({
  country: 'USA',
  distance: {
    amount: 10,
    unit: 'miles',
    mode: 'taxi'
  }
})
console.log(`Your 10-mile taxi trip had a carbon footprint of ${taxiFootprint} kilograms.`)

const fuelFootprint = await carbonFootprint({
  country: 'GBR',
  fuel: {
    amount: 456,
    unit: 'gallons',
    type: 'jetFuel'
  }
})
```
