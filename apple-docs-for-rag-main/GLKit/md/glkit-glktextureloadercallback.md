

- GLKit
-  GLKTextureLoaderCallback 

Type Alias

# GLKTextureLoaderCallback

Signature for the block executed after an asynchronous texture loading operation completes.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
typealias GLKTextureLoaderCallback = (GLKTextureInfo?, (any Error)?) -> Void
```

## Discussion

The block parameters are defined as follows:

*textureInfo*  
A texture info object that describes the loaded texture or `nil` if an error occurred.

*error*  
If the operation was successful, this value is nil; otherwise, this parameter holds an object that describes the problem that occurred.

## See Also

### Constants

Texture Loading Options

Keys to specify in a `textureOperations` dictionary.

Texture Error Handling

Strings used when handling error messages returned from a texture loading method.

enum Code

Values to be returned when a texture loader encounters an error.

