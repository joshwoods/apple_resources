

- SafetyKit
-  SAAuthorizationStatus 

Enumeration

# SAAuthorizationStatus

An enumeration that represents the current Crash Detection event authorization state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
enum SAAuthorizationStatus
```

## Overview

To verify that your app receives Crash Detection events, call requestAuthorization(completionHandler:) and inspect the authorization state.

## Topics

### Obtaining status

case authorized

This is the designated app for receiving Crash Detection events.

case denied

The system denies the app from receiving Crash Detection events because another app has authorization.

case notDetermined

There isn’t a designated app for receiving Crash Detection events.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Detecting a crash

class SACrashDetectionManager

Provides registration and management of Crash Detection events.

class SACrashDetectionEvent

Describes the information about a vehicular crash.

protocol SACrashDetectionDelegate

The protocol that an object adopts to receive Crash Detection events and changes to the authorization status.

