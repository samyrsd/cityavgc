# cityavgc
Get average temperature in celsius of a city.

### How to install
`$ go get github.com/samyrsd/cityavgc`
 
### How to run
You need to have API key from [OpenWeatherMap](https://openweathermap.org) and [APIXU](https://apixu.com) to run this.

`$ cityavgc -owm=1149c95db51fe0344e7d21e58d375368 -axu=34546903e37e4104a3a71758192403`

### How to use
`$ curl localhost:8000/weather/{city}`

Example: `$ curl localhost:8000/weather/tokyo`

### How it works
- Get temperatures from [OpenWeatherMap](https://openweathermap.org) and [APIXU](https://apixu.com) using goroutine
- Average them and return the value in celsius
