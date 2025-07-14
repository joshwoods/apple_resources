

- Vision
- ImageProcessingRequest
-  regionOfInterest 

Instance Property

# regionOfInterest

The region of the image where the framework performs the request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var regionOfInterest: NormalizedRect { get set }
```

**Required**

## Discussion

The system normalizes the rectangle to the dimensions of the processed image. Its origin is the image’s lower-left corner.

The default value is `{ { 0, 0 }, { 1, 1 } }`.

