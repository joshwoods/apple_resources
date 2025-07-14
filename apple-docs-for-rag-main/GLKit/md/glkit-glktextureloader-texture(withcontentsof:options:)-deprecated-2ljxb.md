

- GLKit
- GLKTextureLoader
-  texture(withContentsOf:options:) Deprecated

Type Method

# texture(withContentsOf:options:)

Loads a 2D texture image from a memory range and creates a new texture from the data.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class func texture(
    withContentsOf data: Data,
    options: [String : NSNumber]? = nil
) throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`data`  

The memory range to load as a texture.

`options`  

A dictionary that describes any additional steps you want the texture loader to take when loading the texture. See Texture Loading Options.

## Return Value

A texture info object that describes the loaded texture or `nil` if an error occurred.

## Discussion

This class method loads the texture into the sharegroup attached to the current context for the thread this method is called on.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating Textures from In-Memory Representations

func texture(withContentsOf: Data, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a memory range and creates a new texture from the data.

Deprecated

