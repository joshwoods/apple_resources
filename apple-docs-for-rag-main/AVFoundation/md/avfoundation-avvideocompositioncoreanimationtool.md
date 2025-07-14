

- AVFoundation
-  AVVideoCompositionCoreAnimationTool 

Class

# AVVideoCompositionCoreAnimationTool

An object used to incorporate Core Animation into a video composition.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVVideoCompositionCoreAnimationTool
```

## Overview

Any animations will be interpreted on the video’s timeline, not real-time, so you should:

1.  Set animations’ beginTime property to AVCoreAnimationBeginTimeAtZero rather than `0` (which CoreAnimation replaces with CACurrentMediaTime());

2.  Set isRemovedOnCompletion to false on animations so they are not automatically removed;

3.  Avoid using layers that are associated with UIView objects.

## Topics

### Creating a Composition Tool

convenience init(additionalLayer: CALayer, asTrackID: CMPersistentTrackID)

Adds a Core Animation layer to the video composition.

convenience init(postProcessingAsVideoLayer: CALayer, in: CALayer)

Composes the composited video frame with a Core Animation layer.

convenience init(postProcessingAsVideoLayers: [CALayer], in: CALayer)

Composes the composited video frames with the Core Animation layer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

