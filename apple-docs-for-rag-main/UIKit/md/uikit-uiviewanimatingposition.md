

- UIKit
-  UIViewAnimatingPosition 

Enumeration

# UIViewAnimatingPosition

Constants indicating positions within the animation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
enum UIViewAnimatingPosition
```

## Topics

### Constants

case end

The end point of the animation. Use this constant when you want the final values for any animatable properties—that is, you want to refer to the values you specified in your animation blocks.

case start

The beginning of the animation. Use this constant when you want the starting values for any animatable properties—that is, the values of the properties before you applied any animations.

case current

The current position. Use this constant when you want the most recent value set by an animator object.

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

### Constants

enum UIViewAnimatingState

Constants indicating the current state of the animation.

