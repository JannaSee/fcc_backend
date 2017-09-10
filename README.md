# fcc_backend
back-end projects for free code camp

API Basejump: Timestamp Microservice

User stories:

1. I can pass a string as a parameter, and it will check to see whether that string contains either a unix timestamp or a natural language date (example: January 1, 2016)
2. If it does, it returns both the Unix timestamp and the natural language form of that date.
3. If it does not contain a date or Unix timestamp, it returns null for those properties.
Example usage:

"https://localhost:8080/September%2017,%202017"

"https://timestamp-ms.herokuapp.com/1450137600"

"https://localhost:8080/September2017,092017"

Example output:

{"unix":1505631600,"natural":"September 17, 2017"}

{"unix": 1450137600, "natural":"December 15, 2015"}

{"unix":null,"natural":null}

- Reflections -

This first exercise is not straight forward for those new to back-end. To complete this exercise you need to get node (and express) working on the platform of your choosing. Then write your javascript code. The code passes either a heroku (or similar website) url OR you can use your home computer and pass the localhost url through to the javascript code. See the hint below if you are working on your home computer and get stuck. Finally to check if the code works you need to copy the timestamps into the URL. A JSON formatted timestamp should appear. Try changing the date and the timestamp microservice should adjust the answer.


HINT: app.get('/',function(req, res) { res.send('http://localhost:8080/September%2017,%202017'); //do something })
