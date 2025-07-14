

- AVFAudio
- AVAudioRoutingArbiter
-  AVAudioRoutingArbiter.Category 

Enumeration

# AVAudioRoutingArbiter.Category

Categories that describe the general nature of your app’s audio use.

macOS 11.0+

``` source
enum Category
```

## Overview

The category provides context that helps the operating system arbitrate between Apple devices that are trying to take ownership of a Bluetooth audio route.

## Topics

### Categories

case playback

The app plays audio.

case playAndRecord

The app plays and records audio.

case playAndRecordVoice

The app uses Voice over IP (VoIP).

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

### Participating in AirPods Automatic Switching

func begin(category: AVAudioRoutingArbiter.Category, completionHandler: (Bool, (any Error)?) -> Void)

Begins routing arbitration to take ownership of a nearby Bluetooth audio route.

func leave()

Stops an app’s participation in audio routing arbitration.

