

- Quartz
-  QCPlugInInputImageSource Deprecated

Protocol

# QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

macOS 10.4–10.15Deprecated

``` source
protocol QCPlugInInputImageSource
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

Input images are opaque source objects that comply to this protocol. To create an image input port as an Objective-C 2.0 property, declare it as follows:

```
@property(dynamic) id inputImage;
```

To create an image input port dynamically. use the type `QCPortTypeImage`:

```
[self addInputPortWithType:QCPortTypeImage
                    forKey:@"inputImage"
            withAttributes:nil];
```

## Topics

### Converting an Image to a Representation

func lockTextureRepresentation(with: CGColorSpace!, forBounds: NSRect) -> Bool

Creates an OpenGL texture representation from a subregion of the image source using the provided color space.

**Required**

func unlockTextureRepresentation()

Releases the OpenGL texture representation of the image source.

**Required**

func lockBufferRepresentation(withPixelFormat: String!, colorSpace: CGColorSpace!, forBounds: NSRect) -> Bool

Creates a memory buffer representation from a subregion of the image source using the provided pixel format and color space.

**Required**

func bindTextureRepresentation(toCGLContext: CGLContextObj!, textureUnit: GLenum, normalizeCoordinates: Bool)

Binds the texture to a given texture unit and optionally scales or flips the texture.

**Required**

func unbindTextureRepresentation(fromCGLContext: CGLContextObj!, textureUnit: GLenum)

Unbinds the texture from a texture unit.

**Required**

func unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

**Required**

### Getting Color Space Information

func imageColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image source.

**Required**

func shouldColorMatch() -> Bool

Returns whether or not the image source should be color matched.

**Required**

### Getting Texture Information

func texturePixelsWide() -> Int

Returns the width of the texture representation.

**Required**

func texturePixelsHigh() -> Int

Returns the height of the texture representation.

**Required**

func textureTarget() -> GLenum

Returns the texture target.

**Required**

func textureName() -> GLuint

Returns the texture name.

**Required**

func textureColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the texture representation.

**Required**

func textureFlipped() -> Bool

Returns whether or not the contents of the texture are flipped vertically.

**Required**

func textureMatrix() -> UnsafePointer&lt;GLfloat>!

Returns a texture matrix.

**Required**

### Getting Image Buffer Information

func imageBounds() -> NSRect

Returns the actual bounds of the image source expressed in pixels and aligned to integer boundaries.

**Required**

func bufferPixelsWide() -> Int

Returns the width of the image buffer representation.

**Required**

func bufferPixelsHigh() -> Int

Returns the height of the image buffer representation.

**Required**

func bufferPixelFormat() -> String!

Returns the pixel format of the image buffer representation.

**Required**

func bufferColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image buffer representation.

**Required**

func bufferBaseAddress() -> UnsafeRawPointer!

Returns the base address of the image buffer.

**Required**

func bufferBytesPerRow() -> Int

Returns the bytes per row of the buffer representation.

**Required**

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

protocol QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

Deprecated

