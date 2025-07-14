

- Accelerate
- vImage
- vImage.Size
-  init(cvPixelBuffer:) 

Initializer

# init(cvPixelBuffer:)

Creates a size with dimensions specified by a Core Video pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(cvPixelBuffer: CVPixelBuffer)
```

## Parameters 

`cvPixelBuffer`  

The source Core Video pixel buffer.

## See Also

### Initializers

init?&lt;T>(exactWidth: T, height: T)

Creates a size with dimensions specified as floating-point values.

init?&lt;T>(exactWidth: T, height: T)

Creates a size with dimensions specified as integer values.

init?(exactly: CGSize)

Creates a size with dimensions specified as a Core Graphics size value.

init(width: Int, height: Int)

Creates a size with dimensions specified as integer values.

init(width: vImagePixelCount, height: vImagePixelCount)

Creates a size with dimensions specified as unsigned integer values.

