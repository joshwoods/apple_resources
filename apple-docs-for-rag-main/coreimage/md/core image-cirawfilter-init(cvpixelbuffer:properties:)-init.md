

- Core Image
- CIRAWFilter
-  init(cvPixelBuffer:properties:) 

Initializer

# init(cvPixelBuffer:properties:)

Creates a RAW filter from the pixel buffer and its properties that you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(
    cvPixelBuffer buffer: CVPixelBuffer,
    properties: [AnyHashable : Any]
)
```

## Parameters 

`buffer`  

A Core Video pixel buffer.

`properties`  

A dictionary that defines the properties of the pixel buffer.

## See Also

### Creating a filter

init?(imageData: Data, identifierHint: String?)

Creates a RAW filter from the image data and type hint that you specify.

init?(imageURL: URL)

Creates a RAW filter from the image at the URL location that you specify.

