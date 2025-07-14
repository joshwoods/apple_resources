

- AVFoundation
- AVPlayer
-  AVPlayer.Status 

Enumeration

# AVPlayer.Status

Status values that indicate whether a player can successfully play media.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Status
```

## Topics

### Status Values

case unknown

A value that indicates a player hasn’t attempted to load media for playback.

case readyToPlay

A value that indicates the player is ready to media.

case failed

A value that indicates the player can no longer play media due to an error.

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

### Determining Player Readiness

var status: AVPlayer.Status

A value that indicates the readiness of a player object for playback.

var error: (any Error)?

An error that caused a failure.

