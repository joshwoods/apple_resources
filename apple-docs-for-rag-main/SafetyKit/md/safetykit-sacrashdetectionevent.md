

- SafetyKit
-  SACrashDetectionEvent 

Class

# SACrashDetectionEvent

Describes the information about a vehicular crash.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
class SACrashDetectionEvent
```

## Overview

When a vehicular crash occurs, SafetyKit calls your delegate’s crashDetectionManager(_:didDetect:) method with an SACrashDetectionEvent object. Inspect this object to determine information about the crash, including the date and time, location, and if the system attempted to contact emergency services.

## Topics

### Determining the event type

enum Response

An enumeration that defines possible emergency responses to a Crash Detection event.

var date: Date

The date and time the crash occurred.

var location: CLLocation?

The longitude and latitude where the crash detection occurred.

var response: SACrashDetectionEvent.Response

An indication of whether the system attempted to call an Emergency SOS provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Detecting a crash

class SACrashDetectionManager

Provides registration and management of Crash Detection events.

enum SAAuthorizationStatus

An enumeration that represents the current Crash Detection event authorization state.

protocol SACrashDetectionDelegate

The protocol that an object adopts to receive Crash Detection events and changes to the authorization status.

