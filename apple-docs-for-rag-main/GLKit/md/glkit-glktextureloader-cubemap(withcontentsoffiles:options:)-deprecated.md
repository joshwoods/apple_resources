

- GLKit
- GLKTextureLoader
-  cubeMap(withContentsOfFiles:options:) Deprecated

Type Method

# cubeMap(withContentsOfFiles:options:)

Loads a cube map texture image from a series of files and creates a new texture from the data.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class func cubeMap(
    withContentsOfFiles paths: [Any],
    options: [String : NSNumber]? = nil
) throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`paths`  

An array of URL or `String` objects that provide the paths to the six files that make up the cube map.

`options`  

A dictionary that describes any additional steps you want the texture loader to take when loading the texture. See Texture Loading Options.

## Return Value

A texture info object that describes the loaded texture or `nil` if an error occurred.

## Discussion

The array of file paths must include six entries for the six faces of the cube map. The URLs should be arranged in the following order: Right(+x), Left(-x), Top(+y), Bottom(-y), Front(+z), Back(-z). This coordinate system is left-handed if you think of yourself within the cube. The coordinate system is right-handed if you think of yourself outside of the cube.

This class method loads the texture into the sharegroup attached to the current context for the thread this method is called on.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## Topics

### Related Documentation

func cubeMap(withContentsOf: URL, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a single URL and creates a new texture from the data.

## See Also

### Loading Cube Maps from Files

class func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?) throws -> GLKTextureInfo

Loads a cube map texture image from a single file and creates a new texture from the data.

Deprecated

func cubeMap(withContentsOfFile: String, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a single file and creates a new texture from the data.

Deprecated

func cubeMap(withContentsOfFiles: [Any], options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a cube map texture image from a series of files and creates a new texture from the data.

Deprecated

