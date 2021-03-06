# date2json

[![Greenkeeper badge](https://badges.greenkeeper.io/tigercosmos/date2json.svg)](https://greenkeeper.io/)
[![Build Status](https://travis-ci.org/tigercosmos/date2json.svg?branch=master)](https://travis-ci.org/tigercosmos/date2json)
[![npm version](https://badge.fury.io/js/date2json.svg)](https://badge.fury.io/js/date2json)
[![npm](https://img.shields.io/npm/dt/date2json.svg?style=flat-square)](https://www.npmjs.com/package/date2json)

Parse Date to Json in JavaScript

## Usage

```bash
npm i date2json --save
```

```js
date2json() // Get current time
date2json(new Date()) // Equal to the first one
date2json(new Date(1518545575000)) // Put Date object in the function to get that time
```

```js
const date2json = require("date2json");

const currentTime = date2json();
console.log(currentTime);
// Local time in string JSON format
// {
//   "year": "YYYY",
//   "month": "MM",
//   "day": "DD",
//   "hour": "HH",
//   "minute": "mm",
//   "second": "SS"
// }

const otherTime = date2json(new Date(1518545575000));
console.log(otherTime);
// Local time with the epoch in string JSON format
// {
//   "year": "2018",
//   "month": "02",
//   "day": "14",
//   "hour": "02",
//   "minute": "12",
//   "second": "55"
// }
```

## License

MIT
