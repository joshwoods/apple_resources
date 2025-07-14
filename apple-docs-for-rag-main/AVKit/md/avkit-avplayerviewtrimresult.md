

- AVKit
-  AVPlayerViewTrimResult 

Enumeration

# AVPlayerViewTrimResult

Constants that specify an action a user takes when trimming media in a player view.

macOS 10.9+

``` source
enum AVPlayerViewTrimResult
```

## Topics

### Trim Results

case okButton

The user clicked the Trim button.

case cancelButton

The user clicked the Cancel button.

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

### Trimming Media

var canBeginTrimming: Bool

A Boolean value that indicates whether the player view can begin trimming.

func beginTrimming(completionHandler: ((AVPlayerViewTrimResult) -> Void)?)

Puts the player view into trimming mode.

