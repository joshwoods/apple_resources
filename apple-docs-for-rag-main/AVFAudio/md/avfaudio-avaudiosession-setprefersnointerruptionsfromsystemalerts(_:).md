

- AVFAudio
- AVAudioSession
-  setPrefersNoInterruptionsFromSystemAlerts(\_:) 

Instance Method

# setPrefersNoInterruptionsFromSystemAlerts(\_:)

Sets the preference for not interrupting the audio session with system alerts.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
func setPrefersNoInterruptionsFromSystemAlerts(_ inValue: Bool) throws
```

## Parameters 

`inValue`  

The interruption preference value.

## Mentioned in 

Handling audio interruptions

## Discussion

Beginning in iOS 14, users can set a global preference that indicates whether the system displays incoming calls using a banner or a full-screen display style. If using the banner style, setting this value to true prevents the system from interrupting the audio session with incoming call notifications, and gives the user an opportunity to accept or decline the call. The system only interrupts the audio session if the user accepts the call.

Enabling this preference can improve the user experience of apps with audio sessions that you don’t want to interrupt, such as those that record audiovisual media or that you use for music performance.

Important

This preference has no effect if the device uses the full-screen display style—the system interrupts the audio session on incoming calls.

## See Also

### Handling interruptions

var prefersNoInterruptionsFromSystemAlerts: Bool

A Boolean value that indicates a preference for not interrupting the session with system alerts.

var prefersInterruptionOnRouteDisconnect: Bool

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

func setPrefersInterruptionOnRouteDisconnect(Bool) throws

Sets a preference to interrupt the audio session when the active route disconnects.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

