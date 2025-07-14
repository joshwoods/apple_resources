

- AVFAudio
- AVAudioSession
-  routeChangeNotification 

Type Property

# routeChangeNotification

A notification the system posts when its audio route changes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let routeChangeNotification: NSNotification.Name
```

## Mentioned in 

Responding to audio route changes

## Discussion

The userInfo dictionary of this notification contains the AVAudioSessionRouteChangeReasonKey and AVAudioSessionRouteChangePreviousRouteKey keys, which provide information about the route change.

See Responding to audio route changes for more information on using this notification.

The system posts this notification on a secondary thread.

## Topics

### User Info Keys

let AVAudioSessionRouteChangeReasonKey: String

A user info key that’s used to retrieve the route change reason.

let AVAudioSessionRouteChangePreviousRouteKey: String

A user info key that’s used to retrieve the previously active audio session route.

### User Info Values

enum RouteChangeReason

Constants that indicate the reason for an audio route change.

## See Also

### Inspecting the current route

var currentRoute: AVAudioSessionRouteDescription

A description of the current audio route’s input and output ports.

class AVAudioSessionRouteDescription

An object that describes the input and output ports associated with a session’s audio route.

class AVAudioSessionPortDescription

Information about the capabilities of the port and the hardware channels it supports.

