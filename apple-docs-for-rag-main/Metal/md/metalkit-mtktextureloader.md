

- MetalKit
-  MTKTextureLoader 

Class

# MTKTextureLoader

An object that creates textures from existing data in common image formats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MTKTextureLoader
```

## Overview

Use the MTKTextureLoader class to create a Metal texture from existing image data.

This class supports common file formats, like PNG, JPEG, and TIFF. It also loads image data from KTX and PVR files, asset catalogs, Core Graphics images, and other sources. It infers the output texture format and pixel format from the image data.

You create textures synchronously or asynchronously using MTKTextureLoader methods that return MTLTexture instances. Pass options to these methods that customize the image-loading and texture-creation process.

First create an MTKTextureLoader instance, passing the device that it uses to create textures. Then use one of the texture loader’s methods to create a texture. The code example below synchronously creates a texture from data at a URL, using the default options:

- Swift
- Objective-C

```
func loadTextureUsingMetalKit(url: URL, device: MTLDevice) throws -> MTLTexture {
    let loader = MTKTextureLoader(device: device)

    return try loader.newTexture(URL: url, options: nil)
}
```

```
- (id)loadTextureUsingMetalKit: (NSURL *) url device: (id) device {
    NSError *error;
    MTKTextureLoader *loader = [[MTKTextureLoader alloc] initWithDevice: device];

    id texture = [loader newTextureWithContentsOfURL:url options:nil error:&error];

    if(!texture)
    {
        NSLog(@"Error creating the texture from %@: %@", url.absoluteString, error.localizedDescription);
        return nil;
    }
    return texture;
}
```

If you use custom data formats, or change the image data at runtime, use MTLTexture methods instead. For more information, see Creating and Sampling Textures.

## Topics

### Creating a Texture Loader

init(device: any MTLDevice)

Initializes a new texture loader object.

var device: any MTLDevice

The device object that the texture loader uses to create textures.

### Loading Textures from URLs

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given URL.

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given URL.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, error: NSErrorPointer) -> [any MTLTexture]

Synchronously loads image data and creates new Metal textures from the specified list of URLs.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates new Metal textures from the specified list of URLs.

### Loading Textures from Asset Catalogs

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTextures(names: [String], scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog, using a specified display gamut.

func newTexture(name: String, scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTextures(names: [String], scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

### Loading Textures from Core Graphics Images

func newTexture(cgImage: CGImage, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given bitmap image.

func newTexture(cgImage: CGImage, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given bitmap image.

### Loading Textures from In-Memory Data Representations

func newTexture(data: Data, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously creates a new Metal texture from an in-memory representation of the texture’s data.

func newTexture(data: Data, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously creates a new Metal texture from an in-memory representation of the texture’s data.

### Loading Textures from Model I/O Representations

func newTexture(texture: MDLTexture, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the specified Model I/O texture.

func newTexture(texture: MDLTexture, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the specified Model I/O texture.

### Specifying Loading Options

struct Option

Keys and values used to specify loading options.

### Completing a Texture Loading Operation

typealias ArrayCallback

The signature for the block executed after an asynchronous loading operation for multiple textures has completed.

typealias Callback

The signature for the block executed after an asynchronous loading operation for a single texture has completed.

### Handling Errors

struct Error

Errors returned by the texture loader.

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

