

- GLKit
- GLKTextureLoader
-  texture(with:options:) Deprecated

Type Method

# texture(with:options:)

Loads a 2D texture image from a Quartz image and creates a new texture from the data.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class func texture(
    with cgImage: CGImage,
    options: [String : NSNumber]? = nil
) throws -> GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`cgImage`  

The Quartz image to be turned into a texture.

`options`  

A dictionary that describes any additional steps you want the texture loader to take when loading the texture. See Texture Loading Options.

## Return Value

A texture info object that describes the loaded texture or `nil` if an error occurred.

## Discussion

This class method loads the texture into the sharegroup attached to the current context for the thread this method is called on.

If the image was created using the CGBitmapImageContextCreate function, it must use one of the pixel formats described in the table below. CGImages loaded from files typically are already in one of these formats.

| Color Space | Pixel format and bitmap information constant |
|----|----|
| Null | 8 bpp, 8 bpc, CGImageAlphaInfo.alphaOnly |
| Gray | 8 bpp, 8 bpc, CGImageAlphaInfo.none |
| Gray | 8 bpp, 8 bpc, CGImageAlphaInfo.alphaOnly |
| RGB | 32 bpp, 8 bpc, CGImageAlphaInfo.noneSkipFirst |
| RGB | 32 bpp, 8 bpc, CGImageAlphaInfo.premultipliedFirst |

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating Textures from CGImages

func texture(with: CGImage, options: [String : NSNumber]?, queue: dispatch_queue_t?, completionHandler: GLKTextureLoaderCallback)

Asynchronously loads a 2D texture image from a Quartz image and creates a new texture from the data.

Deprecated

