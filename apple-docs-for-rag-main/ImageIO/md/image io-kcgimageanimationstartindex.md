

- Image I/O
-  kCGImageAnimationStartIndex 

Global Variable

# kCGImageAnimationStartIndex

A property that specifies the index of the first frame of an animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let kCGImageAnimationStartIndex: CFString
```

## Discussion

The value of this property is a CFNumber that contains an unsigned integer. To override the start index value in the image file, include this property in the options dictionary when animating an image.

## See Also

### Animations

func CGAnimateImageAtURLWithBlock(CFURL, CFDictionary?, CGImageSourceAnimationBlock) -> OSStatus

Animate the sequence of images in the Graphics Interchange Format (GIF) or Animated Portable Network Graphics (APNG) file at the specified URL.

func CGAnimateImageDataWithBlock(CFData, CFDictionary?, CGImageSourceAnimationBlock) -> OSStatus

Animate the sequence of images using data from a Graphics Interchange Format (GIF) or Animated Portable Network Graphics (APNG) file file.

typealias CGImageSourceAnimationBlock

The block to execute for each frame of an image animation.

let kCGImageAnimationDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImageAnimationLoopCount: CFString

The number of times to repeat the animated sequence.

enum CGImageAnimationStatus

Constants that indicate the result of animating an image sequence.

