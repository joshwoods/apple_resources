

- Accelerate
- vImage
- vImage.Size
-  init(width:height:) 

Initializer

# init(width:height:)

Creates a size with dimensions specified as integer values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    width: Int,
    height: Int
)
```

## Parameters 

`width`  

The width.

`height`  

The height.

## Discussion

The height and width must be greater than `0`.

## See Also

### Initializers

init(cvPixelBuffer: CVPixelBuffer)

Creates a size with dimensions specified by a Core Video pixel buffer.

init?&lt;T>(exactWidth: T, height: T)

Creates a size with dimensions specified as floating-point values.

init?&lt;T>(exactWidth: T, height: T)

Creates a size with dimensions specified as integer values.

init?(exactly: CGSize)

Creates a size with dimensions specified as a Core Graphics size value.

init(width: vImagePixelCount, height: vImagePixelCount)

Creates a size with dimensions specified as unsigned integer values.

