

- AVFoundation
- AVVideoCompositing
-  supportsHDRSourceFrames 

Instance Property

# supportsHDRSourceFrames

A Boolean value that indicates whether the compositor handles source frames that contain high dynamic range (HDR) properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
optional var supportsHDRSourceFrames: Bool { get }
```

## See Also

### Inspecting Processing Requirements

var sourcePixelBufferAttributes: [String : any Sendable]?

The pixel buffer attributes that the compositor accepts for source frames.

**Required**

var requiredPixelBufferAttributesForRenderContext: [String : any Sendable]

The pixel buffer attributes that the compositor requires for pixel buffers that it creates.

**Required**

var supportsWideColorSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contains wide color properties.

var canConformColorOfSourceFrames: Bool

A Boolean value that indicates whether the compositor conforms the color space of source frames to the composition color space.

