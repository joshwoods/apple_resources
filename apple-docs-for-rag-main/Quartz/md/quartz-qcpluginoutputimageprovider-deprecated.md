

- Quartz
-  QCPlugInOutputImageProvider Deprecated

Protocol

# QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

macOS 10.4–10.15Deprecated

``` source
protocol QCPlugInOutputImageProvider
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

Output images are opaque provider objects that comply to this protocol. To create an image output port as an Objective-C 2.0 property, declare it as follows:

```
@property(dynamic) id outputImage;
```

To create an image input port dynamically use the type `QCPortTypeImage`:

```
[self addOutputPortWithType:QCPortTypeImage
                    forKey:@"outputImage"
            withAttributes:nil];
```

To write images to that port, you need to implement the methods in this protocol and create an internal class that represents the images produced by the custom patch. For example, a simple interface for an image provider is:

```
@interface MyOutputImage : NSObject 
{
    NSUInteger _width;
    NSUInteger _height;
}
```

## Topics

### Rendering an Image to a Destination

func render(toBuffer: UnsafeMutableRawPointer!, withBytesPerRow: Int, pixelFormat: String!, forBounds: NSRect) -> Bool

Renders a subregion of the image into the supplied memory buffer using the specified pixel format.

func copyRenderedTexture(forCGLContext: CGLContextObj!, pixelFormat: String!, bounds: NSRect, isFlipped: UnsafeMutablePointer&lt;ObjCBool>!) -> GLuint

Returns the name of an OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that contains a subregion of the image in a given pixel format.

func render(withCGLContext: CGLContextObj!, forBounds: NSRect) -> Bool

Renders a subregion of the image to the provided CGL context.

func releaseRenderedTexture(GLuint, forCGLContext: CGLContextObj!)

Releases the previously copied texture.

### Providing Information About the Image

func imageBounds() -> NSRect

Returns the bounds of the image expressed in pixels and aligned to integer boundaries.

**Required**

func imageColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image or `NULL` if the image should not be color matched.

**Required**

func shouldColorMatch() -> Bool

Returns whether the image should be color matched.

### Providing Information About the Rendering Destination

func supportedBufferPixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to a memory buffer.

func supportedRenderedTexturePixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to an onscreen OpenGL context.

func canRender(withCGLContext: CGLContextObj!) -> Bool

Returns whether the image data can be rendered into the provided CGL context.

## See Also

### Protocols

QCCompositionParameterViewDelegate

A protocol for composition parameter view’s delegate.

QCCompositionPickerViewDelegate

The `QCCompositionPickerViewDelegate` informal protocol defines methods that allow your application to respond to changes in a composition picker view (a QCCompositionPickerView object).

protocol QCCompositionRenderer

The `QCRenderer` protocol defines the methods used to pass data to the input ports or retrieve data from the output ports of the root patch of a Quartz Composer composition. This protocol is adopted by the QCRenderer, QCView, and QCCompositionLayer classes.

Deprecated

protocol QCPlugInContext

The `QCPlugInContext` protocol defines methods that you use only from within the execution method (execute(_:atTime:withArguments:)) of a `QCPlugIn` object.

Deprecated

protocol QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

Deprecated

