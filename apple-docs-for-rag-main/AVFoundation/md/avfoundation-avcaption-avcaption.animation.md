

- AVFoundation
- AVCaption
-  AVCaption.Animation 

Enumeration

# AVCaption.Animation

Animation options for a caption.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Animation
```

## Topics

### Animations

case none

No animation.

case characterReveal

A character reveal animation.

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

### Accessing Animation

var animation: AVCaption.Animation

The animation that the system applies to this caption.

