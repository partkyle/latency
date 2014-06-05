# Latency App

Written in Go and deployed on Heroku (http://peaceful-falls-6706.herokuapp.com/), this app returns a json message after a random delay (between 0 and 9 seconds). You can specify the delay with `?delay=n`, where `n` is an integer.

To get a list of urls, http://peaceful-falls-6706.herokuapp.com/sample. Optionally, pass use the `n` parameter to set the number of returned urls: http://peaceful-falls-6706.herokuapp.com/sample?n=20

You can also set the type of response directly to ```json```, ```xml```, or ```txt``` with the following:
* http://peaceful-falls-6706.herokuapp.com/json/sample
* http://peaceful-falls-6706.herokuapp.com/xml/sample
* http://peaceful-falls-6706.herokuapp.com/txt/sample

You can run locally with `PORT=9999 go run latency.go`. If you have issues with `go get` for the uuid resource, you can manually clone it in to the `src/github.com/nu7hatch` directory
