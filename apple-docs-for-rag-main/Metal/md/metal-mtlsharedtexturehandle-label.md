

- Metal
- MTLSharedTextureHandle
-  label 

Instance Property

# label

A string that identifies the texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
var label: String? { get }
```

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Shared Texture Handle

var device: any MTLDevice

The device object that created the texture.

