

- Core Image
- CIRAWFilter
-  init(imageData:identifierHint:) 

Initializer

# init(imageData:identifierHint:)

Creates a RAW filter from the image data and type hint that you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(
    imageData data: Data,
    identifierHint: String?
)
```

## Parameters 

`data`  

The image data.

`identifierHint`  

A string that identifies the image type.

## See Also

### Creating a filter

init?(cvPixelBuffer: CVPixelBuffer, properties: [AnyHashable : Any])

Creates a RAW filter from the pixel buffer and its properties that you specify.

init?(imageURL: URL)

Creates a RAW filter from the image at the URL location that you specify.

