

- AVFoundation
- AVVideoCompositing
-  sourcePixelBufferAttributes 

Instance Property

# sourcePixelBufferAttributes

The pixel buffer attributes that the compositor accepts for source frames.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var sourcePixelBufferAttributes: [String : any Sendable]? { get }
```

**Required**

## Discussion

The property is required to provide a kCVPixelBufferPixelFormatTypeKey key in the dictionary, along with attributes for which the compositor needs specific values to work properly. Omitted attributes will be supplied by the composition engine to allow for the best performance. If the attribute kCVPixelBufferPixelFormatTypeKey key is not in the dictionary an exception will be raised. The value of the kCVPixelBufferPixelFormatTypeKey is an array of `kCVPixelFormatType_*` constants as defined in Pixel_Format_Types.

If the custom compositor is meant to be used with an AVVideoCompositionCoreAnimationTool created using the init(additionalLayer:asTrackID:) method, kCVPixelFormatType_32BGRA should be included as one of the supported pixel format types.

Missing attributes will be set by the composition engine to values allowing the best performance.

This property is queried once before any composition request is sent to the compositor. Changing source buffer attributes afterwards is not supported.

## See Also

### Inspecting Processing Requirements

var requiredPixelBufferAttributesForRenderContext: [String : any Sendable]

The pixel buffer attributes that the compositor requires for pixel buffers that it creates.

**Required**

var supportsHDRSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contain high dynamic range (HDR) properties.

var supportsWideColorSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contains wide color properties.

var canConformColorOfSourceFrames: Bool

A Boolean value that indicates whether the compositor conforms the color space of source frames to the composition color space.

