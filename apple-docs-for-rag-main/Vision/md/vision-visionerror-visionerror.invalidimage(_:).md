

- Vision
- VisionError
-  VisionError.invalidImage(\_:) 

Case

# VisionError.invalidImage(\_:)

An error that indicates the input image is invalid.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
case invalidImage(String)
```

## Discussion

This error occurs when you pass an invalid image to an operation, like passing an image with no dimensions.

## See Also

### Getting the invalid error

case invalidArgument(String)

An error that indicates a request has an invalid value.

case invalidFormat(String)

An error that indicates a request has data that’s formatted incorrectly.

case invalidModel(String)

An error that indicates the Core ML model isn’t compatible with the request.

case invalidOperation(String)

An error that indicates an app requests an unsupported operation.

