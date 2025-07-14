

- AVFAudio
- AVAudioSession
-  AVAudioSession.RouteSelection 

Enumeration

# AVAudioSession.RouteSelection

Constants used to define the active route selection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum RouteSelection
```

## Topics

### Constants

case none

No route is selected.

case local

The local device is selected.

case external

An external device is selected.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Preparing for long-form video playback

func prepareRouteSelectionForPlayback(completionHandler: (Bool, AVAudioSession.RouteSelection) -> Void)

Prepares the route selection for long-form video playback.

