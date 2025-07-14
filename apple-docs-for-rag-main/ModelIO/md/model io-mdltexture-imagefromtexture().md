

- Model I/O
- MDLTexture
-  imageFromTexture() 

Instance Method

# imageFromTexture()

Exports the texture data as a CoreGraphics image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func imageFromTexture() -> Unmanaged?
```

## Return Value

A CoreGraphics image object containing the texture’s pixel data, or `nil` if the texture data cannot be represented using CoreGraphics.

## See Also

### Exporting Textures

func write(to: URL) -> Bool

Exports the texture data to an image file at the specified URL.

func write(to: URL, type: CFString) -> Bool

Exports the texture data to an image file at the specified URL, of the specified type.

