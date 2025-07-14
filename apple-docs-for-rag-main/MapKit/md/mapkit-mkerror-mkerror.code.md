

- MapKit
- MKError
-  MKError.Code 

Enumeration

# MKError.Code

Error constants for the MapKit framework.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
enum Code
```

## Topics

### Constants

case decodingFailed

GeoJSON decoding failed.

case directionsNotFound

The framework couldn’t find the specified directions.

case loadingThrottled

The data didn’t load because data throttling is in effect.

case placemarkNotFound

The specified placemark could not be found.

case serverFailure

The map server was unable to return the desired information.

case unknown

An unknown error occurred.

case decodingFailed

GeoJSON decoding failed.

case directionsNotFound

The framework couldn’t find the specified directions.

case loadingThrottled

The data didn’t load because data throttling is in effect.

case placemarkNotFound

The specified placemark could not be found.

case serverFailure

The map server was unable to return the desired information.

case unknown

An unknown error occurred.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

let MKErrorDomain: String

The error domain for MapKit.

struct MKError

Error constants for the MapKit framework.

