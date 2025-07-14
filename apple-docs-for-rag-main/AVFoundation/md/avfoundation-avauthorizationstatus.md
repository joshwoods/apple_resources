

- AVFoundation
-  AVAuthorizationStatus 

Enumeration

# AVAuthorizationStatus

Constants that indicate the status of an app’s authorization to capture media.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
enum AVAuthorizationStatus
```

## Overview

Call authorizationStatus(for:) to determine the app’s current permission to capture media.

## Topics

### Status Values

case notDetermined

A status that indicates the user hasn’t yet granted or denied authorization.

case restricted

A status that indicates the app isn’t permitted to use media capture devices.

case denied

A status that indicates the user has explicitly denied an app permission to capture media.

case authorized

A status that indicates the user has explicitly granted an app permission to capture media.

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

### Authorizing Device Access

class func requestAccess(for: AVMediaType, completionHandler: (Bool) -> Void)

Requests the user’s permission to allow the app to capture media of a particular type.

class func authorizationStatus(for: AVMediaType) -> AVAuthorizationStatus

Returns an authorization status that indicates whether the user grants the app permission to capture media of a particular type.

