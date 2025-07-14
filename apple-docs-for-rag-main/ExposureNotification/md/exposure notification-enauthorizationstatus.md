

- Exposure Notification
-  ENAuthorizationStatus 

Enumeration

# ENAuthorizationStatus

A set of cases that indicates the authorization status for the app.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
enum ENAuthorizationStatus
```

## Overview

Important

This enumeration is available in iOS 12.5, and in iOS 13.5 and later.

## Topics

### Authorization States

case authorized

Authorization is granted.

case notAuthorized

Authorization is denied.

case restricted

Authorization is restricted.

case unknown

Authorization is not determined.

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

### Status

enum ENStatus

A set of cases that represents the overall status of exposure notification on the system.

