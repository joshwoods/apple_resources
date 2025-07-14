

- AVFAudio
- AVAudioSession
-  prefersInterruptionOnRouteDisconnect 

Instance Property

# prefersInterruptionOnRouteDisconnect

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var prefersInterruptionOnRouteDisconnect: Bool { get }
```

## Discussion

The default value is true.

## See Also

### Handling interruptions

var prefersNoInterruptionsFromSystemAlerts: Bool

A Boolean value that indicates a preference for not interrupting the session with system alerts.

func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws

Sets the preference for not interrupting the audio session with system alerts.

func setPrefersInterruptionOnRouteDisconnect(Bool) throws

Sets a preference to interrupt the audio session when the active route disconnects.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

