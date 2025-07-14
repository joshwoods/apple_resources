

- App Tracking Transparency
-  ATTrackingManager 

Class

# ATTrackingManager

A class that provides a tracking authorization request and the tracking authorization status of the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class ATTrackingManager
```

## Topics

### Requesting Authorization

class func requestTrackingAuthorization(completionHandler: (ATTrackingManager.AuthorizationStatus) -> Void)

The request for user authorization to access app-related data.

### Determining Tracking Authorization Status

class var trackingAuthorizationStatus: ATTrackingManager.AuthorizationStatus

The authorization status that is current for the calling application.

enum AuthorizationStatus

The status values for app tracking authorization.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

