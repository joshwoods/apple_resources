

- WatchKit
-  WKAudioFilePlayerItemStatus Deprecated

Enumeration

# WKAudioFilePlayerItemStatus

Constants that represent the status of a player item.

watchOS 2.0–6.0Deprecated

``` source
enum WKAudioFilePlayerItemStatus
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Topics

### Statuses

case unknown

The item’s status is unknown.

case readyToPlay

The item is ready to play.

case failed

The item can’t be played.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

