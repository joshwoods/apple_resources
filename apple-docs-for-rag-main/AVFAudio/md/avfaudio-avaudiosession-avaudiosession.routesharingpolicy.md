

- AVFAudio
- AVAudioSession
-  AVAudioSession.RouteSharingPolicy 

Enumeration

# AVAudioSession.RouteSharingPolicy

Cases that indicate the possible route-sharing policies for an audio session.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum RouteSharingPolicy
```

## Overview

A route-sharing policy allows you to specify that an audio session should route its output to somewhere other than the default system output when alternative routes are available.

## Topics

### Route-sharing policies

case `default`

A policy that follows standard rules for routing audio output.

case longFormAudio

A policy that routes output to the shared long-form audio output.

case longFormVideo

A policy that routes output to the shared long-form video output.

case independent

A policy in which the route picker UI directs videos to a wireless route.

static var longForm: AVAudioSession.RouteSharingPolicy

A policy that routes output to the shared long-form audio output.

Deprecated

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the route sharing policy

var routeSharingPolicy: AVAudioSession.RouteSharingPolicy

The active route-sharing policy.

