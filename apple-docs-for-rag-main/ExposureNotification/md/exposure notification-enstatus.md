

- Exposure Notification
-  ENStatus 

Enumeration

# ENStatus

A set of cases that represents the overall status of exposure notification on the system.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
enum ENStatus
```

## Overview

Important

This enumeration is available in iOS 12.5, and in iOS 13.5 and later.

## Topics

### States

case active

Notification is active.

case bluetoothOff

Bluetooth is turned off.

case disabled

Notification is disabled.

case restricted

Notification is not active due to system restrictions, such as parental controls.

case unknown

Notification is unknown.

case paused

The user paused Exposure Notification.

case unauthorized

The user hasn’t authorized Exposure Notification.

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

enum ENAuthorizationStatus

A set of cases that indicates the authorization status for the app.

