

- SafetyKit
-  SACrashDetectionDelegate 

Protocol

# SACrashDetectionDelegate

The protocol that an object adopts to receive Crash Detection events and changes to the authorization status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
protocol SACrashDetectionDelegate : NSObjectProtocol
```

## Overview

Upon app launch, immediately set the delegate so it receives Crash Detection events. If the app isn’t running, the system launches it in the background and then sends the event.

## Topics

### Obtaining a Crash Detection event

func crashDetectionManager(SACrashDetectionManager, didDetect: SACrashDetectionEvent)

Receive and process a Crash Detection event.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Detecting a crash

class SACrashDetectionManager

Provides registration and management of Crash Detection events.

enum SAAuthorizationStatus

An enumeration that represents the current Crash Detection event authorization state.

class SACrashDetectionEvent

Describes the information about a vehicular crash.

