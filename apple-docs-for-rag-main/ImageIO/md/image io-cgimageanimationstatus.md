

- Image I/O
-  CGImageAnimationStatus 

Enumeration

# CGImageAnimationStatus

Constants that indicate the result of animating an image sequence.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CGImageAnimationStatus
```

## Topics

### Animation Status

case allocationFailure

case corruptInputImage

case incompleteInputImage

case parameterError

case unsupportedFormat

### Initializers

init?(rawValue: OSStatus)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Animations

func CGAnimateImageAtURLWithBlock(CFURL, CFDictionary?, CGImageSourceAnimationBlock) -> OSStatus

Animate the sequence of images in the Graphics Interchange Format (GIF) or Animated Portable Network Graphics (APNG) file at the specified URL.

func CGAnimateImageDataWithBlock(CFData, CFDictionary?, CGImageSourceAnimationBlock) -> OSStatus

Animate the sequence of images using data from a Graphics Interchange Format (GIF) or Animated Portable Network Graphics (APNG) file file.

typealias CGImageSourceAnimationBlock

The block to execute for each frame of an image animation.

let kCGImageAnimationStartIndex: CFString

A property that specifies the index of the first frame of an animation.

let kCGImageAnimationDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImageAnimationLoopCount: CFString

The number of times to repeat the animated sequence.

