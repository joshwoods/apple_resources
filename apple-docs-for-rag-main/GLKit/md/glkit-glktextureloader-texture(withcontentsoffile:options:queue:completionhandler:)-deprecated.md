

- GLKit
- GLKTextureLoader
-  texture(withContentsOfFile:options:queue:completionHandler:) Deprecated

Instance Method

# texture(withContentsOfFile:options:queue:completionHandler:)

Asynchronously loads a 2D texture image from a file and creates a new texture from the data.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
func texture(
    withContentsOfFile path: String,
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?,
    completionHandler block: @escaping GLKTextureLoaderCallback
)
```

``` source
func texture(
    withContentsOfFile path: String,
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?
) async throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`path`  

A path to the file to load.

`options`  

A dictionary that describes any additional steps you want the texture loader to take when loading the texture. See Texture Loading Options.

`queue`  

A dispatch queue that your block is called on when the task completes. If `NULL` is passed, the block is called on the main dispatch queue.

`block`  

A block to be called when the task completes.

## Discussion

This method is identical to texture(withContentsOfFile:options:), except that it loads the texture asynchronously. When this method is called, it creates a new background task to handle the request and then returns control to your app. Later, when the task is complete, GLKit calls your completion handler on the queue you provided.

## See Also

### Loading Textures from Files

class func texture(withContentsOfFile: String, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a 2D texture image from a file and creates a new texture from the data.

Deprecated

