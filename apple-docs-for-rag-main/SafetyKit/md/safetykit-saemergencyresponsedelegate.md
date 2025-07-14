

- SafetyKit
-  SAEmergencyResponseDelegate 

Protocol

# SAEmergencyResponseDelegate

The interface for receiving updates about a requested emergency response action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
protocol SAEmergencyResponseDelegate : NSObjectProtocol
```

## Topics

### Receiving voice call status

func emergencyResponseManager(SAEmergencyResponseManager, didUpdateVoiceCallStatus: SAEmergencyResponseManager.VoiceCallStatus)

Provides the voice call status to the delegate.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to a crash

class SAEmergencyResponseManager

Provides actions in response to a Crash Detection event.

enum Response

An enumeration that defines possible emergency responses to a Crash Detection event.

