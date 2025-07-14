

- Cinematic
-  CNRenderingSession 

Class

# CNRenderingSession

An object representing the context in which rendering occurs.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNRenderingSession
```

## Topics

### Structures

struct Attributes

The rendering session asset attributes.

struct FrameAttributes

Controls the focus distance and aperture of the rendering for the frames.

### Initializers

init(commandQueue: any MTLCommandQueue, sessionAttributes: CNRenderingSession.Attributes, preferredTransform: CGAffineTransform, quality: CNRenderingQuality)

Intializes an object for a rendering session.

### Instance Properties

let commandQueue: any MTLCommandQueue

The command queue of a Metal device that creates the command buffer.

let preferredTransform: CGAffineTransform

The preferred transform of the rendered image for display purposes.

let quality: CNRenderingQuality

The quality of rendering desired for a session.

let sessionAttributes: CNRenderingSession.Attributes

Rendering session attributes for a Cinematic asset.

### Instance Methods

func encodeRender(to: any MTLCommandBuffer, frameAttributes: CNRenderingSession.FrameAttributes, sourceImage: CVPixelBuffer, sourceDisparity: CVPixelBuffer, destinationImage: CVPixelBuffer) -> Bool

func encodeRender(to: any MTLCommandBuffer, frameAttributes: CNRenderingSession.FrameAttributes, sourceImage: CVPixelBuffer, sourceDisparity: CVPixelBuffer, destinationLuma: any MTLTexture, destinationChroma: any MTLTexture) -> Bool

func encodeRender(to: any MTLCommandBuffer, frameAttributes: CNRenderingSession.FrameAttributes, sourceImage: CVPixelBuffer, sourceDisparity: CVPixelBuffer, destinationRGBA: any MTLTexture) -> Bool

### Type Properties

static var destinationPixelFormatTypes: [OSType]

A static number representing the video compositor’s required pixel buffer attributes context dictionary when implementing video compositing.

static var sourcePixelFormatTypes: [OSType]

The static pixel format types supported for the output destination.

## See Also

### Reading and rendering

class CNAssetInfo

An object that provides Cinematic-specific information about an asset, including its tracks.

class CNCompositionInfo

An object that enables you to add the appropriate number of tracks for a Cinematic asset.

