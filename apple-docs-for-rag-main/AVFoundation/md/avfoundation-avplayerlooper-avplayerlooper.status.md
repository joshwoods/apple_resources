

- AVFoundation
- AVPlayerLooper
-  AVPlayerLooper.Status 

Enumeration

# AVPlayerLooper.Status

Status constants that indicate whether a looper can successfully perform looping playback.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum Status
```

## Topics

### Status Values

case unknown

The status isn’t known.

case ready

The looper is ready to perform looping playback.

case failed

The looper isn’t able to perform looping playback due to an error.

case cancelled

The app canceled looping on the player.

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

### Observing Looping State

var loopCount: Int

The number of times the object played the media.

var status: AVPlayerLooper.Status

A status that indicates the object’s ability to loop playback.

