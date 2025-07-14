

- GLKit
- GLKTextureLoader
-  texture(withName:scaleFactor:bundle:options:queue:completionHandler:) Deprecated

Instance Method

# texture(withName:scaleFactor:bundle:options:queue:completionHandler:)

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
func texture(
    withName name: String,
    scaleFactor: CGFloat,
    bundle: Bundle?,
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?,
    completionHandler block: @escaping GLKTextureLoaderCallback
)
```

``` source
func texture(
    withName name: String,
    scaleFactor: CGFloat,
    bundle: Bundle?,
    options: [String : NSNumber]? = nil,
    queue: dispatch_queue_t?
) async throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

