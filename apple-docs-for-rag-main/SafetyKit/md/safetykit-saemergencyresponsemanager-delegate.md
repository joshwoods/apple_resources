

- SafetyKit
- SAEmergencyResponseManager
-  delegate 

Instance Property

# delegate

The object that receives voice call status updates and requested emergency response actions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
weak var delegate: (any SAEmergencyResponseDelegate)? { get set }
```

## See Also

### Placing a voice call

enum VoiceCallStatus

An enumeration that defines the status of a requested voice call.

func dialVoiceCall(toPhoneNumber: String, completionHandler: (Bool, (any Error)?) -> Void)

Request the system to dial a voice call on behalf of someone involved in a crash.

