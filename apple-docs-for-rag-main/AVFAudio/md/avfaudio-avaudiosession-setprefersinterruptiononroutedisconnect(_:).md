

- AVFAudio
- AVAudioSession
-  setPrefersInterruptionOnRouteDisconnect(\_:) 

Instance Method

# setPrefersInterruptionOnRouteDisconnect(\_:)

Sets a preference to interrupt the audio session when the active route disconnects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func setPrefersInterruptionOnRouteDisconnect(_ inValue: Bool) throws
```

## Parameters 

`inValue`  

Specify a false value to opt out of interruption on route disconnect. Set to true to reset to the default behavior.

## Discussion

The expected behavior of an app is to pause playback if a route change occurs due to a device no longer being available (AVAudioSession.RouteChangeReason.oldDeviceUnavailable). Starting in iOS 17, the system interrupts active Now Playing sessions when a route change occurs due to a disconnection event, but doesn’t interrupt other sessions.

## See Also

### Handling interruptions

var prefersNoInterruptionsFromSystemAlerts: Bool

A Boolean value that indicates a preference for not interrupting the session with system alerts.

func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws

Sets the preference for not interrupting the audio session with system alerts.

var prefersInterruptionOnRouteDisconnect: Bool

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

