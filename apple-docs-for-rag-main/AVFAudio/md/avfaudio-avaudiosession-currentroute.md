

- AVFAudio
- AVAudioSession
-  currentRoute 

Instance Property

# currentRoute

A description of the current audio route’s input and output ports.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currentRoute: AVAudioSessionRouteDescription { get }
```

## Mentioned in 

Responding to audio route changes

## Discussion

An audio route is an electronic pathway for audio signals. Inspect the state of device audio routes and configure your preferred input and output route settings.

## See Also

### Inspecting the current route

class AVAudioSessionRouteDescription

An object that describes the input and output ports associated with a session’s audio route.

class AVAudioSessionPortDescription

Information about the capabilities of the port and the hardware channels it supports.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

