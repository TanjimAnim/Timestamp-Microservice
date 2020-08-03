
# API Project: Timestamp Microservice for FCC

### User stories:

1. The API endpoint is `GET https://timestamp-micrevice.glitch.me/api/timestamp/:date_string?`
2. If the date string is **empty** the api returns the current timestamp.
3. If the date string is **valid** the api returns a JSON having the structure
   `{"unix": <date.getTime()>, "utc" : <date.toUTCString()> }`
   e.g. `{"unix": 1479663089000 ,"utc": "Sun, 20 Nov 2016 17:31:29 GMT"}`.
4. If the date string is **invalid** the api returns a JSON having the structure `{"error" : "Invalid Date" }`.

#### Example usage:

- https://timestamp-micrevice.glitch.me/api/timestamp/2015-12-25
- https://timestamp-micrevice.glitch.me/api/timestamp/1451001600000

#### Example output:

- {"unix":1451001600000, "utc":"Fri, 25 Dec 2015 00:00:00 GMT"}
