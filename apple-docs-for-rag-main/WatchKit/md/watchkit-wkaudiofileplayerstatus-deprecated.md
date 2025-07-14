

- WatchKit
-  WKAudioFilePlayerStatus Deprecated

Enumeration

# WKAudioFilePlayerStatus

Constants that represent the status of the player.

watchOS 2.0–6.0Deprecated

``` source
enum WKAudioFilePlayerStatus
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Topics

### Constants

case unknown

The status of the item is unknown because the player has not yet loaded the audio file for playback.

case readyToPlay

The player is ready to play its item.

case failed

The player can no longer play the audio because of an error. Use the error property to get information about the error that occurred.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

