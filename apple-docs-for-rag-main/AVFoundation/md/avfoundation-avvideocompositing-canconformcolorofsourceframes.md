

- AVFoundation
- AVVideoCompositing
-  canConformColorOfSourceFrames 

Instance Property

# canConformColorOfSourceFrames

A Boolean value that indicates whether the compositor conforms the color space of source frames to the composition color space.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
optional var canConformColorOfSourceFrames: Bool { get }
```

## Discussion

A custom compositor indicates its processing requirements through the sourcePixelBufferAttributes and supportsWideColorSourceFrames properties. By default, the composition engine prepares source frames by converting them to meet the compositor’s configuration.

When this property value is true, the engine doesn’t convert source pixel buffers that meet the compositor’s processing requirements. However, it does convert buffers that don’t meet the processing requirements, which includes the following cases:

- The values of supportsWideColorSourceFrames and supportsHDRSourceFrames are false, but the source buffers contain wide color. In this case, the engine converts the color space of source pixel buffers to BT.709 color space. Note that when supportsHDRSourceFrames is true, the engine also assumes supportsWideColorSourceFrames is true.

- The value of supportsHDRSourceFrames is false and source buffers contain HDR color. In this case, the engine converts the color space of source pixel buffers to the composition color space.

- The pixel format of the source buffers isn’t specified in sourcePixelBufferAttributes. In this case, the engine converts the pixel format to a supported format and converts the color space to the composition color space.

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

var supportsWideColorSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contains wide color properties.

