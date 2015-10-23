# Promised Trello

Small wrapper for node-trello that uses promises and self explaining functions
to access the API.

Right now there are only GET-functions available, but I will add more.

## Install

```
npm install promised-trello
```

## Example
```
var Trello = require('promised-trello');

var t = new Trello(<key>, <token>);

t.getMyBoards().then(function(data) {
  console.log(JSON.stringify(data));
})
.catch(function (error) {
    // Handle any error from all above steps
    console.log('Error:');
    console.log(error);
})
.done();
```
