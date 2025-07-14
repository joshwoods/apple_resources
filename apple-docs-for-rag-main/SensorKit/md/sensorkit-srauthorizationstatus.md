

- SensorKit
-  SRAuthorizationStatus 

Enumeration

# SRAuthorizationStatus

The states that model whether the user approves the app to read a particular sensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum SRAuthorizationStatus
```

## Topics

### Enumeration Cases

case authorized

User has granted authorization to this application

case denied

User has denied authorization to this application or data collection is disabled in Settings.

case notDetermined

User has not yet made a choice regarding this application

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

### Checking user authorization

var authorizationStatus: SRAuthorizationStatus

The status of the user’s agreement to let the app access this reader’s sensor.

class func requestAuthorization(sensors: Set&lt;SRSensor>, completion: ((any Error)?) -> Void)

Requests user permission to read one or more sensors.

