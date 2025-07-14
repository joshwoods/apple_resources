

- MapKit
- MKDirections
-  MKDirections.RoutePreference 

Enumeration

# MKDirections.RoutePreference

Options that modify how the framework selects routes when calculating directions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum RoutePreference
```

## Topics

### Route selection options

case any

The option that specifies any available route.

case avoid

The option that requests the framework avoid certain routes.

case any

The option that specifies any available route.

case avoid

The option that requests the framework avoid certain routes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a directions object

init(request: MKDirections.Request)

Creates and returns a directions object using the specified request.

class Request

The start and end points of a route, along with the planned mode of transportation.

