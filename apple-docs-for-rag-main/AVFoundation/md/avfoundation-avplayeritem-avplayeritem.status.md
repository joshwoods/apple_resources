

- AVFoundation
- AVPlayerItem
-  AVPlayerItem.Status 

Enumeration

# AVPlayerItem.Status

The statuses for a player item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Status
```

## Topics

### Player Item Statuses

case unknown

The item’s status is unknown.

case readyToPlay

The item is ready to play.

case failed

The item no longer plays due to an error.

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

### Determining Readiness

var status: AVPlayerItem.Status

The status of the player item.

var error: (any Error)?

The error that caused the player item to fail.

