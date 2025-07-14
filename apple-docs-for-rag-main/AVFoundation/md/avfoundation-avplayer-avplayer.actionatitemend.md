

- AVFoundation
- AVPlayer
-  AVPlayer.ActionAtItemEnd 

Enumeration

# AVPlayer.ActionAtItemEnd

The actions a player can take when it finishes playing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum ActionAtItemEnd
```

## Topics

### Actions

case advance

The player should advance to the next item, if there is one.

case pause

The player should pause playing.

case none

The player should do nothing.

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

### Responding When Playback Ends

var actionAtItemEnd: AVPlayer.ActionAtItemEnd

The action to perform when the current player item has finished playing.

