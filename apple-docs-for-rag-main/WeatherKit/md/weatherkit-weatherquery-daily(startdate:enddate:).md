

- WeatherKit
- WeatherQuery
-  daily(startDate:endDate:) 

Type Method

# daily(startDate:endDate:)

Returns weather for an arbitrary range of days, with the following caveats:

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func daily(
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

A daily forecast query for the specified time range

## Discussion

- Historical data is available from Aug 1, 2021.

- Forecasts are available up to 10 days in the future.

- Each request will return a maximum of 10 days.

- A day is included in the forecast if midnight in local time is included in the range of `startDate` (inclusive) to `endDate` (exclusive).

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

static func hourly(startDate: Date, endDate: Date) -> WeatherQuery&lt;T>

The hourly forecast query that takes a start date and end date for the request, with the following caveats:

