

- Model I/O
- MDLTexture
-  write(to:type:) 

Instance Method

# write(to:type:)

Exports the texture data to an image file at the specified URL, of the specified type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func write(
    to nsurl: URL,
    type: CFString
) -> Bool
```

## Parameters 

`nsurl`  

The file URL at which to write the texture image.

`type`  

A Uniform Type Identifier declaring the image file format to use for export.

## Return Value

true if export succeeded; false otherwise.

## Discussion

For the `type` parameter, pass the Uniform Type Identifier for any output format supported by the Image I/O framework, such as the JPEG, TIFF, PNG, or (in macOS only) OpenEXR format. For details, see Uniform Type Identifiers Reference.

## See Also

### Exporting Textures

func write(to: URL) -> Bool

Exports the texture data to an image file at the specified URL.

func imageFromTexture() -> Unmanaged&lt;CGImage>?

Exports the texture data as a CoreGraphics image.

