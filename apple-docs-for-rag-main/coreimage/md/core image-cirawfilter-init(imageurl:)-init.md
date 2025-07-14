

- Core Image
- CIRAWFilter
-  init(imageURL:) 

Initializer

# init(imageURL:)

Creates a RAW filter from the image at the URL location that you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(imageURL url: URL)
```

## Parameters 

`url`  

The URL location of the image.

## See Also

### Creating a filter

init?(cvPixelBuffer: CVPixelBuffer, properties: [AnyHashable : Any])

Creates a RAW filter from the pixel buffer and its properties that you specify.

init?(imageData: Data, identifierHint: String?)

Creates a RAW filter from the image data and type hint that you specify.

