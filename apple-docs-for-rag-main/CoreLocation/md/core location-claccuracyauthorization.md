

- Core Location
-  CLAccuracyAuthorization 

Enumeration

# CLAccuracyAuthorization

Constants that indicate the level of location accuracy the app has authorization to use.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CLAccuracyAuthorization
```

## Topics

### Getting the location accuracy

case fullAccuracy

The user authorized the app to access location data with full accuracy.

case reducedAccuracy

The user authorized the app to access location data with reduced accuracy.

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

### Authorization

Requesting authorization to use location services

Obtain authorization to use location services and manage changes to your app’s authorization status.

Suspending authorization requests

Defer the system’s authorization request dialog until your app is ready.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

Deprecated

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

Deprecated

