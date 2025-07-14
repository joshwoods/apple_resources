

- SafetyKit
- SAEmergencyResponseDelegate
-  emergencyResponseManager(\_:didUpdateVoiceCallStatus:) 

Instance Method

# emergencyResponseManager(\_:didUpdateVoiceCallStatus:)

Provides the voice call status to the delegate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
optional func emergencyResponseManager(
    _ emergencyResponseManager: SAEmergencyResponseManager,
    didUpdateVoiceCallStatus voiceCallStatus: SAEmergencyResponseManager.VoiceCallStatus
)
```

**Required**

## Parameters 

`emergencyResponseManager`  

The emergency response object responsible for the status update.

`voiceCallStatus`  

The status of the voice call.

## Discussion

A voice call to the desired contact can occur when running in the foreground or background within a limited time window of a Crash Detection event. Use this delegate method to monitor the status of the requested voice call.

