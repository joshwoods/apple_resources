

- Video Subscriber Account
-  VSCheckAccessOption 

Structure

# VSCheckAccessOption

The options your app uses when checking access status.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
struct VSCheckAccessOption
```

## Topics

### Options

static let prompt: VSCheckAccessOption

A Boolean that indicates whether your app can prompt the user to grant access.

### Creating check access options

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking Access Status

func checkAccessStatus(options: [VSCheckAccessOption : Any], completionHandler: (VSAccountAccessStatus, (any Error)?) -> Void)

Checks your app’s access to user subscription information, and requests access if needed.

enum VSAccountAccessStatus

Constants that represent your app’s access status to the user’s subscription information.

