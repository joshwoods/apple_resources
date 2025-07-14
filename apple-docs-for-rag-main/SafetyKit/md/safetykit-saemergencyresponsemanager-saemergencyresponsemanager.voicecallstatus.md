

- SafetyKit
- SAEmergencyResponseManager
-  SAEmergencyResponseManager.VoiceCallStatus 

Enumeration

# SAEmergencyResponseManager.VoiceCallStatus

An enumeration that defines the status of a requested voice call.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
enum VoiceCallStatus
```

## Topics

### Determining call status

case active

The system successfully placed a call to the desired contact and that call is currently active.

case dialing

The system is dialing the desired contact.

case disconnected

The voice call to the desired contact disconnected.

case failed

The voice call failed to connect to the desired contact.

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

### Placing a voice call

func dialVoiceCall(toPhoneNumber: String, completionHandler: (Bool, (any Error)?) -> Void)

Request the system to dial a voice call on behalf of someone involved in a crash.

var delegate: (any SAEmergencyResponseDelegate)?

The object that receives voice call status updates and requested emergency response actions.

