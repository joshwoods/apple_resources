

- GLKit
-  GLKTextureLoader Deprecated

Class

# GLKTextureLoader

A utility class that simplifies loading OpenGL or OpenGL ES texture datas from a variety of image file formats.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKTextureLoader
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

The GLKTextureLoader class can load two-dimensional or cubemap textures in most image formats supported by the Image I/O framework. In iOS, it can also load textures compressed in the PVRTC format. It can load the data synchronously or asynchronously.

To load textures synchronously, make a context with the desired sharegroup the current context, and then call one or more of the class methods. The returned texture info object includes details about the loaded texture.

To load textures asynchronously, your initialization code allocates and initializes a new GLKTextureLoader object using the sharegroup object that should be the destination for new textures. Then, to load a texture, your app calls one of the texture loader’s instance methods, passing in a completion handler block to be called when the texture has been loaded.

The following OpenGL properties are set for a newly created, non-mipmapped texture:

- `GL_TEXTURE_MIN_FILTER`:`GL_LINEAR`

- `GL_TEXTURE_MAG_FILTER`:`GL_LINEAR`

- `GL_TEXTURE_WRAP_S`:`GL_CLAMP_TO_EDGE`

- `GL_TEXTURE_WRAP_T`:`GL_CLAMP_TO_EDGE`

The following OpenGL properties are set for a newly created, mipmapped texture:

- `GL_TEXTURE_MIN_FILTER`:`GL_LINEAR_MIPMAP_LINEAR`

- `GL_TEXTURE_MAG_FILTER`:`GL_LINEAR`

- `GL_TEXTURE_WRAP_S`:`GL_CLAMP_TO_EDGE`

- `GL_TEXTURE_WRAP_T`:`GL_CLAMP_TO_EDGE`

The `GLKTextureLoader` and `GLKTextureInfo` classes do not manage the OpenGL texture for you. Once the texture is returned to your app, you are responsible for it. This means that after your app is finished using an OpenGL texture, it must explicitly deallocate it by calling the `glDeleteTextures` function.

## Topics

### Initialization

init(sharegroup: EAGLSharegroup)

Initializes a new texture loader object.

init(share: NSOpenGLContext)

Initializes a new texture loader object.

### Loading Textures from Files

class func texture(withContentsOfFile: String, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a 2D texture image from a file and creates a new texture from the data.

func texture(withContentsOfFile: String, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a file and creates a new texture from the data.

### Loading a Texture From a URL

class func texture(withContentsOf: URL, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a 2D texture image from a URL and creates a new texture from the data.

func texture(withContentsOf: URL, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a URL and creates a new texture from the data.

### Creating Textures from In-Memory Representations

class func texture(withContentsOf: Data, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a 2D texture image from a memory range and creates a new texture from the data.

func texture(withContentsOf: Data, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a memory range and creates a new texture from the data.

### Creating Textures from CGImages

class func texture(with: CGImage, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a 2D texture image from a Quartz image and creates a new texture from the data.

func texture(with: CGImage, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a Quartz image and creates a new texture from the data.

### Loading Cube Maps from Files

class func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a single file and creates a new texture from the data.

func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a single file and creates a new texture from the data.

class func cubeMap(withContentsOfFiles: [Any], options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a series of files and creates a new texture from the data.

func cubeMap(withContentsOfFiles: [Any], options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a series of files and creates a new texture from the data.

### Loading Cube Maps from URLs

class func cubeMap(withContentsOf: URL, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a single URL and creates a new texture from the data.

func cubeMap(withContentsOf: URL, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a single URL and creates a new texture from the data.

### Constants

typealias GLKTextureLoaderCallback

Signature for the block executed after an asynchronous texture loading operation completes.

Texture Loading Options

Keys to specify in a `textureOperations` dictionary.

Texture Error Handling

Strings used when handling error messages returned from a texture loading method.

enum Code

Values to be returned when a texture loader encounters an error.

### Instance Methods

func texture(withName: String, scaleFactor: CGFloat, bundle: Bundle?, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

### Type Methods

class func texture(withName: String, scaleFactor: CGFloat, bundle: Bundle?, options: [String : NSNumber]?) throws -> GLKTextureInfo

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

## See Also

### Texture Loading

class GLKTextureInfo

Information about OpenGL textures created by the GLKTextureLoader class.

Deprecated

