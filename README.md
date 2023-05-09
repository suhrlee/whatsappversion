## About




## API Request

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
const url = 'http://localhost/whatsappversion/index.json'
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
