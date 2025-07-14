

- AVFoundation
- AVVideoCompositing
-  supportsWideColorSourceFrames 

Instance Property

# supportsWideColorSourceFrames

A Boolean value that indicates whether the compositor handles source frames that contains wide color properties.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional var supportsWideColorSourceFrames: Bool { get }
```

## Mentioned in 

Tagging Media with Video Color Information

## See Also

### Inspecting Processing Requirements

var sourcePixelBufferAttributes: [String : any Sendable]?

The pixel buffer attributes that the compositor accepts for source frames.

**Required**

var requiredPixelBufferAttributesForRenderContext: [String : any Sendable]

The pixel buffer attributes that the compositor requires for pixel buffers that it creates.

**Required**

var supportsHDRSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contain high dynamic range (HDR) properties.

var canConformColorOfSourceFrames: Bool

A Boolean value that indicates whether the compositor conforms the color space of source frames to the composition color space.

