## About




## API Request

`request(url, options, (error, res, body) => {
    if (error) {
        return  console.log(error)
    };

    if (!error && res.statusCode == 200) {
        console.log(body)
    };
});`


`axios.post(url2,{
    headers: {
      Accept: "application/json",
      "Content-Type": "application/json",
    },
  })
  .then(({data}) => {
    console.log(data);
});`
