

- AVFAudio
- AVAudioSession
-  routeSharingPolicy 

Instance Property

# routeSharingPolicy

The active route-sharing policy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 5.0+

``` source
var routeSharingPolicy: AVAudioSession.RouteSharingPolicy { get }
```

## Discussion

Use this value to indicate that the system should route this app’s audio somewhere other than the default system output when other suitable alternative routes exist.

## See Also

### Inspecting the route sharing policy

enum RouteSharingPolicy

Cases that indicate the possible route-sharing policies for an audio session.

