

- Model I/O
- MDLTexture
-  texelDataWithTopLeftOrigin() 

Instance Method

# texelDataWithTopLeftOrigin()

Returns the texture’s image data, organized such that its first pixel represents the top-left corner of the image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func texelDataWithTopLeftOrigin() -> Data?
```

## Return Value

The texture’s image data, or `nil` if data is not available.

## Discussion

If the texture was initialized with image data in bottom-left-origin format, the first call to this method creates and caches image data in top-left-origin format.

This method returns `nil` if the texture was not initialized with image data and is not a MDLTexture subclass capable of loading or generating its own data.

## See Also

### Accessing Texture Data

func texelDataWithBottomLeftOrigin() -> Data?

Returns the texture’s image data, organized such that its first pixel represents the bottom-left corner of the image.

func texelDataWithTopLeftOrigin(atMipLevel: Int, create: Bool) -> Data?

Returns the texture’s image data for the specified mipmap level, organized such that its first pixel represents the top-left corner of the image.

func texelDataWithBottomLeftOrigin(atMipLevel: Int, create: Bool) -> Data?

Returns the texture’s image data for the specified mipmap level, organized such that its first pixel represents the bottom-left corner of the image.

