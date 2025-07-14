

- SafetyKit
-  SAEmergencyResponseManager 

Class

# SAEmergencyResponseManager

Provides actions in response to a Crash Detection event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
class SAEmergencyResponseManager
```

## Overview

Use the manager to place a voice call to an emergency contact upon receipt of a Crash Detection event. Provide an object that adopts SAEmergencyResponseDelegate in order to respond to the status of the voice call.

## Topics

### Placing a voice call

enum VoiceCallStatus

An enumeration that defines the status of a requested voice call.

func dialVoiceCall(toPhoneNumber: String, completionHandler: (Bool, (any Error)?) -> Void)

Request the system to dial a voice call on behalf of someone involved in a crash.

var delegate: (any SAEmergencyResponseDelegate)?

The object that receives voice call status updates and requested emergency response actions.

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

## See Also

### Responding to a crash

protocol SAEmergencyResponseDelegate

The interface for receiving updates about a requested emergency response action.

enum Response

An enumeration that defines possible emergency responses to a Crash Detection event.

