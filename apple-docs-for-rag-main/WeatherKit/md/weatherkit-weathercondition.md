

- WeatherKit
-  WeatherCondition 

Enumeration

# WeatherCondition

A description of the current weather condition.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum WeatherCondition
```

## Topics

### Creating the object

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting visibility properties

case blowingDust

Blowing dust or sandstorm.

case clear

Clear.

case cloudy

Cloudy, overcast conditions.

case foggy

Fog.

case haze

Haze.

case mostlyClear

Mostly clear.

case mostlyCloudy

Mostly cloudy.

case partlyCloudy

Partly cloudy.

case smoky

Smoky.

### Getting wind properties

case breezy

Breezy, light wind.

case windy

Windy.

### Getting precipitation properties

case drizzle

Drizzle or light rain.

case heavyRain

Heavy rain.

case isolatedThunderstorms

Thunderstorms covering less than 1/8 of the forecast area.

case rain

Rain.

case sunShowers

Rain with visible sun.

case scatteredThunderstorms

Numerous thunderstorms spread across up to 50% of the forecast area.

case strongStorms

Notably strong thunderstorms.

case thunderstorms

Thunderstorms.

### Getting hazardous properties

case frigid

Frigid conditions, low temperatures, or ice crystals.

case hail

Hail.

case hot

High temperatures.

### Getting winter precipitation properties

case flurries

Flurries or light snow.

case sleet

Sleet.

case snow

Snow.

case sunFlurries

Snow flurries with visible sun.

case wintryMix

Wintry mix.

### Getting hazardous winter properties

case blizzard

Blizzard.

case blowingSnow

Blowing or drifting snow.

case freezingDrizzle

Freezing drizzle or light rain.

case freezingRain

Freezing rain.

case heavySnow

Heavy snow.

### Getting tropical hazard properties

case hurricane

Hurricane.

case tropicalStorm

Tropical storm.

### Describing the weather condition

var accessibilityDescription: String

A localized accessibility description describing the weather condition.

var description: String

A localized string describing the current condition.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [WeatherCondition]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Characteristics

enum Precipitation

The form of precipitation.

enum PressureTrend

The atmospheric pressure change over time.

struct UVIndex

The expected intensity of ultraviolet radiation from the sun.

struct Wind

Contains wind data of speed, direction, and gust.

