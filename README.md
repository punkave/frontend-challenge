## P'unk Avenue frontend challenge

Using HTML, CSS, and one of the following:

* Vanilla JavaScript
* jQuery

Create a single-page website/web application that displays bike share and weather information for people in Philadelphia using [Indego](https://www.rideindego.com) and [Open Weather Map](https://openweathermap.org/current#name) APIs.

## Requirements

The app:
* Asks the user for an address (you may use an input field)
* Displays the location of at least three nearby bike stations on a map (you may integrate Google Maps, Open Street Map, or another tool of your choice)
* Visually indicates the number of open docks and available bikes at each bike station
* Visually indicates the weather, and
* Displays a warning if the weather seems dangerous.

## APIs
[Indego](https://www.rideindego.com) is Philadelphia's bike-sharing program, with many bike stations in the city.

The [Indego GeoJSON station status API](https://www.rideindego.com/stations/json/) provides a realtime snapshot of the number of bikes available, number of open docks available (not currently containing a bike), and total number of docks at every station. This API is free and requires no API key.

> Hint: the API responds with a JSON object. You may find it easier to work out how to work with the data if you visit the API manually first and feed its output through a [JSON pretty printer](http://jsonprettyprint.com/) or similar tool. **Your actual app should access the API on its own.**

The [Open Weather Map API](https://openweathermap.org/current#name) provides a realtime snapshot of the current weather in a given city. Since Philadelphia is a small geographical area it is sufficient to obtain the weather for a geographical location central to Philadelphia. This API has a free plan, you will need to sign up for an API key. This API is well documented.

## Criteria

Your work will be evaluated primarily on:

* Consistency of coding style (ideally in harmony with our [JavaScript style guide](https://github.com/punkave/best-practices/blob/master/javascript.md))
* Idiomatic use of your chosen JavaScript library (or vanilla JavaScript)
* Good user experience (UX)
* General quality of code and technical communication.

## How to submit your work

Fork this project on github. When you're finished, send us the URL of your public repository. You should also include clear instructions to run the app and/or the URL of your running instance of the app (if you're hosting it). *Consider using `.gitignore` to avoid putting any deployment credentials or API key in your public repository.*

**If you prefer, you may submit your code to us privately by email,** rather than using a fork in your public github.

## Extra credit

* Host it:
  * Make your app available on a server that we can communicate with from the office, not just running it locally. Although this is not a system administration job, we're interested in seeing that you are comfortable with the fundamentals of making something live on a webserver. (Hint: Heroku, Now, Digital Ocean and Linode are all options to consider.)
* Ask the user whether they are looking for a bike, or a place to park one.
* Use color or some other means to emphasize when there are plenty of bikes/racks, or very few.
* Update in real time.
* Geolocation. (Hint: you must use https on your server, which takes some doing.)
* Anything else you think is cool, relevant, and consistent with the other requirements.

## If you don't finish

We are most interested in your frontend development skills. If you have trouble with the APIs, focus first on building the application that would display that data, using mocked-up data at first, and add in real queries to the APIs at the end.
