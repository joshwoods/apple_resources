

- RealityKit
-  TextureResource 

Class

# TextureResource

A representation of a texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class TextureResource
```

## Overview

A texture resource holds pixel data accessible by the GPU, organized as an image, a cube of images, an array of images, or a 3D image (volume texture).

Assign texture resources to material parameters to provide color and fine surface-rendering details.

## Topics

### Creating a texture resource

convenience init(from: LowLevelTexture) throws

Synchronously creates a texture resource from a low-level texture.

convenience init(from: LowLevelTexture) async throws

Asynchronously creates a texture resource from a low-level texture.

struct Contents

An object that references the pixel data for each mipmap level of a texture.

struct Format

The pixel format and encoding of a texture.

struct Compression

The compression to apply when importing an image as a texture.

### Creating a 2D texture resource

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D texture resource from a pixel Metal buffer, or data.

struct Dimensions2D

The dimensions of a 2D texture.

### Creating a cube texture resource

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from a 2D image of cube faces.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from a 2D image of cube faces.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a cube texture resource from face images.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a cube texture resource from face images.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a cube texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

struct DimensionsCube

The dimensions of the cube texture.

### Creating a 2D array texture resource

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 2D texture array by generating it from images.

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 2D texture array by generating it from images.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

struct Dimensions2DArray

The dimensions of the 2D array texture.

### Creating a 3D texture resource

static func texture3D(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 3D texture by generating it from images.

static func texture3D(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 3D texture by generating it from images.

convenience init(dimensions: TextureResource.Dimensions3D, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 3D texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions3D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 3D texture resource from a pixel Metal buffer, or data.

struct Dimensions3D

The dimensions of the 3D texture.

### Loading a texture

convenience init(named: String, in: Bundle?) async throws

Asynchronously loads a texture resource from a bundle.

convenience init(named: String, in: Bundle?, options: TextureResource.CreateOptions) async throws

Asynchronously loads a texture resource from a bundle with options.

convenience init(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a texture resource from a file URL with creation options.

convenience init(contentsOf: URL, withName: String?) async throws

Synchronously creates a texture resource from a file URL.

static func load(named: String, in: Bundle?) throws -> TextureResource

Returns a texture resource by synchronously loading it from a bundle.

static func load(named: String, in: Bundle?, options: TextureResource.CreateOptions) throws -> TextureResource

Returns a texture resource by synchronously loading it from a bundle with options.

static func load(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously loads a texture resource from a URL with options.

static func load(contentsOf: URL, withName: String?) throws -> TextureResource

Synchronously loads a texture resource from a URL.

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle.

Deprecated

static func loadAsync(named: String, in: Bundle?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle with options.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;TextureResource>

Asynchronously loads a texture resource from a URL.

Deprecated

### Describing the texture

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

var pixelFormat: MTLPixelFormat

The texture’s pixel format.

var height: Int

The height of the texture image, in pixels.

var width: Int

The width of the texture image, in pixels.

var depth: Int

The depth of the texture image, in pixels.

var arrayLength: Int

The number of slices in the texture array.

var mipmapLevelCount: Int

The number of mipmaps for the texture.

var semantic: TextureResource.Semantic?

The intended usage of the texture resource.

### Drawing the texture

var drawableQueue: TextureResource.DrawableQueue?

The drawable queue that replaces the texture.

### Copying the texture

func copy(to: any MTLTexture) async throws

Asynchronously copies texture data to another texture.

func copy(to: any MTLTexture) throws

Copies texture data to another texture.

func copyAsync(to: any MTLTexture, completionHandler: ((any Error)?) -> Void)

Asynchronously copies texture data to another texture.

Deprecated

### Modifying the texture

func replace(withDrawables: TextureResource.DrawableQueue)

Dynamically replaces the texture with a drawable queue.

func replace(withImage: CGImage, options: TextureResource.CreateOptions) throws

Dynamically replaces the texture with a Core Graphics image.

func replace(using: CGImage, options: TextureResource.CreateOptions) async throws

Asynchronously replaces the texture with a Core Graphics image.

func replace(with: LowLevelTexture)

Replaces a texture resource with a low-level texture.

### Deprecated

static func generate(from: CGImage, withName: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a texture resource from an in-memory Core Graphics image.

Deprecated

static func generateAsync(from: CGImage, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

func replaceAsync(withImage: CGImage, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously replaces the texture with a Core Graphics image.

Deprecated

static func generate(from: CGImage, named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously loads a texture resource from a URL with options.

Deprecated

### Classes

class Drawable

A drawable associated with a drawable queue

class DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

### Structures

struct CreateOptions

An object that holds texture resource creation options.

### Type Aliases

typealias SamplingQuality

An object for controlling the texture-sampling quality.

### Enumerations

enum MipmapsMode

An enumeration for specifying how to allocate and generate mipmaps for a texture.

enum Semantic

An object for specifying the intended use of a texture.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Resource
- Sendable

## See Also

### Texture resources

struct CreateOptions

An object that holds texture resource creation options.

typealias SamplingQuality

An object for controlling the texture-sampling quality.

enum MipmapsMode

An enumeration for specifying how to allocate and generate mipmaps for a texture.

enum Semantic

An object for specifying the intended use of a texture.

