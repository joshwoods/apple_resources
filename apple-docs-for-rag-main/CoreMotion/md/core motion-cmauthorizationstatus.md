

- Core Motion
-  CMAuthorizationStatus 

Enumeration

# CMAuthorizationStatus

The authorization status for motion-related features.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 4.0+

``` source
enum CMAuthorizationStatus
```

## Topics

### Enumeration Cases

case notDetermined

The status has not yet been determined.

case restricted

Access is denied due to system-wide restrictions.

case denied

Access was denied by the user.

case authorized

Access was granted by the user.

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

### Determining Altitude Availability

class func isAbsoluteAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device reports changes in the absolute altitude.

class func isRelativeAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve altimeter data.

