

- MapKit
-  MKDirectionsTransportType 

Structure

# MKDirectionsTransportType

Constants that specify the type of conveyance to use.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
struct MKDirectionsTransportType
```

## Topics

### Transport types

static var automobile: MKDirectionsTransportType

Directions suitable for use while driving.

static var walking: MKDirectionsTransportType

Directions suitable for a pedestrian.

static var transit: MKDirectionsTransportType

Directions suitable for public transportation.

static var any: MKDirectionsTransportType

Directions suitable for any transportation option.

### Creating direction transport types

init(rawValue: UInt)

Creates a direction transport type using a raw unsigned integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

