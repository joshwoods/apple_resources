

- AVFAudio
- AVAudioSession
-  prefersNoInterruptionsFromSystemAlerts 

Instance Property

# prefersNoInterruptionsFromSystemAlerts

A Boolean value that indicates a preference for not interrupting the session with system alerts.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
var prefersNoInterruptionsFromSystemAlerts: Bool { get }
```

## See Also

### Handling interruptions

func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws

Sets the preference for not interrupting the audio session with system alerts.

var prefersInterruptionOnRouteDisconnect: Bool

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

func setPrefersInterruptionOnRouteDisconnect(Bool) throws

Sets a preference to interrupt the audio session when the active route disconnects.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

