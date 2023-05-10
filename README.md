## About


## Endpoint
```
https://api.whatsversion.com/
```

## Examples

``` js
const request = require('request');
let url = "https://api.whatsversion.com/";
let options = {json: true};
request(url, options, (error, res, body) => {
    if (error) {
        return  console.log(error)
    };
    if (!error && res.statusCode == 200) {
        console.log(body)
    };
});
```

``` js
const axios = require('axios')
const url = 'https://api.whatsversion.com/'
axios.post(url,{
    headers: {
      Accept: "application/json",
      "Content-Type": "application/json",
    },
  })
  .then(({data}) => {
    console.log(data);
});
```

## Structure of Response

``` json
{
    "lastverification": "YYYY-MM-DD HH:MM:SS",
    "web": {
        "latest": "<version>",
        "beta": "<version>"
    },
    "windows": {
        "latest": "<version>",
        "beta": "<version>"
    },
    "macos": {
        "latest": "<version>",
        "beta": "<version>"
    },
    "android": {
        "messenger": "<version>",
        "business": "<version>"
    },
    "ios": {
        "messenger": "<version>",
        "business": "<version>"
    }
}
```
