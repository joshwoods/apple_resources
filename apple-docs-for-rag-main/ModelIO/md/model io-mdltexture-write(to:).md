

- Model I/O
- MDLTexture
-  write(to:) 

Instance Method

# write(to:)

Exports the texture data to an image file at the specified URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func write(to URL: URL) -> Bool
```

## Parameters 

`URL`  

The file URL at which to write the texture image.

## Return Value

true if export succeeded; false otherwise.

## Discussion

Model I/O automatically infers the file format in which to export the image from the filename extension of the `url` parameter. This method can export textures in JPEG, TIFF, PNG, or (in macOS only) OpenEXR format.

## See Also

### Exporting Textures

func write(to: URL, type: CFString) -> Bool

Exports the texture data to an image file at the specified URL, of the specified type.

func imageFromTexture() -> Unmanaged&lt;CGImage>?

Exports the texture data as a CoreGraphics image.

