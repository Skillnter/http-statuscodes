# http-status-codes

All HTTP Status Codes.

## Installation

```console
npm install http-response-status-code
```

## Usage 

```javascript
var STATUS_CODES = require('http-response-status-code');

console.log(STATUS_CODES.getStatusName(STATUS_CODES.OK));
// OK

console.log(STATUS_CODES.getStatusDescription(STATUS_CODES.INTERNAL_SERVER_ERROR));
// Server Error

console.log(STATUS_CODES.getStatusCode("I'm a teapot"));
// 418


res.status(STATUS_CODES.INTERNAL_SERVER_ERROR).end()
res.status(STATUS_CODES.BAD_REQUEST).send(STATUS_CODES.getStatusDescription(400));
res.status(STATUS_CODES.getStatusCode("NOT_FOUND")).sendFile('/absolute/path/to/404.png');
```
