

- Video Subscriber Account
-  VSAccountAccessStatus 

Enumeration

# VSAccountAccessStatus

Constants that represent your app’s access status to the user’s subscription information.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
enum VSAccountAccessStatus
```

## Topics

### Statuses

case denied

The user denied the app access to subscription information.

case granted

The user allowed the app to access subscription information.

case notDetermined

The user hasn’t chosen whether to allow the app to access subscription information.

case restricted

The app isn’t allowed to access subscription information.

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

### Checking Access Status

func checkAccessStatus(options: [VSCheckAccessOption : Any], completionHandler: (VSAccountAccessStatus, (any Error)?) -> Void)

Checks your app’s access to user subscription information, and requests access if needed.

struct VSCheckAccessOption

The options your app uses when checking access status.

