

- WeatherKit
- WeatherQuery
-  hourly(startDate:endDate:) 

Type Method

# hourly(startDate:endDate:)

The hourly forecast query that takes a start date and end date for the request, with the following caveats:

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func hourly(
    startDate: Date,
    endDate: Date
) -> WeatherQuery
```

Available when `T` is `Forecast`.

## Parameters 

`startDate`  

The lower boundary of the time range for the forecast (inclusive)

`endDate`  

The upper boundary of the time range for the forecast (exclusive)

## Return Value

An hourly forecast query for the specified time range

## Discussion

- Historical data is available from Aug 1, 2021.

- Forecasts are available up to 10 days (~240 hours) in the future.

- Each request will return a maximum of 10 days (~240 hours).

- Hours in the forecast range from `startDate`(inclussive) to `endDate` (exclusive)

## See Also

### Creating queries

static var alerts: WeatherQuery&lt;[WeatherAlert]?>

The weather alerts query.

static var availability: WeatherQuery&lt;WeatherAvailability>

The availability query.

static var current: WeatherQuery&lt;CurrentWeather>

The current weather query.

static var daily: WeatherQuery&lt;Forecast&lt;DayWeather>>

The daily forecast query. This returns 10 contiguous days, beginning with the current day.

static var hourly: WeatherQuery&lt;Forecast&lt;HourWeather>>

The hourly forecast query. This returns 25 contiguous hours, beginning with the current hour.

static var minute: WeatherQuery&lt;Forecast&lt;MinuteWeather>?>

The minute forecast query.

static func daily(startDate: Date, endDate: Date) -> WeatherQuery&lt;T>

Returns weather for an arbitrary range of days, with the following caveats:

