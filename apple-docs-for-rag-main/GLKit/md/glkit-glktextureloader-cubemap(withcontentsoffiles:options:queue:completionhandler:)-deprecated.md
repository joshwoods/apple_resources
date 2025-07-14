

- GLKit
- GLKTextureLoader
-  cubeMap(withContentsOfFiles:options:queue:completionHandler:) Deprecated

Instance Method

# cubeMap(withContentsOfFiles:options:queue:completionHandler:)

Asynchronously loads a cube map texture image from a series of files and creates a new texture from the data.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
func cubeMap(
    withContentsOfFiles paths: [Any],
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?,
    completionHandler block: @escaping GLKTextureLoaderCallback
)
```

``` source
func cubeMap(
    withContentsOfFiles paths: [Any],
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?
) async throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`paths`  

An array of paths to the six files that make up the cube map.

`options`  

A dictionary that describes any additional steps you want the texture loader to take when loading the texture. See Texture Loading Options.

`queue`  

A dispatch queue that your block is called on when the task completes. If `NULL` is passed, the block is called on the main dispatch queue.

`block`  

A block to be called when the task completes.

## Discussion

This method is identical to cubeMap(withContentsOf:options:), except that it loads the texture asynchronously. When this method is called, it creates a new background task to handle the request and then returns control to your app. Later, when the task is complete, GLKit calls your completion handler on the queue you provided.

## See Also

### Loading Cube Maps from Files

class func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a single file and creates a new texture from the data.

Deprecated

func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a single file and creates a new texture from the data.

Deprecated

class func cubeMap(withContentsOfFiles: [Any], options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a series of files and creates a new texture from the data.

Deprecated

