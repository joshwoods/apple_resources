

- Image Playground
- ImageCreator
- ImageCreator.Error
-  ImageCreator.Error.unavailable 

Case

# ImageCreator.Error.unavailable

An error that indicates image creation is currently unavailable.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
case unavailable
```

## Discussion

This error can occur if the device doesn’t yet have the models it needs to complete the request.

## See Also

### Getting the error codes

case notSupported

An error that indicates the device doesn’t support image generation.

case creationCancelled

An error that occurs in response to cancellation of the parent task.

case faceInImageTooSmall

An error that indicates the system cannot use one of the source images because the face in it is too small.

case unsupportedLanguage

An error that indicates the input text uses an unsupported language.

case unsupportedInputImage

An error that indicates the system cannot use one of the specified source images.

case backgroundCreationForbidden

An error that indicates the app is hidden or in the background.

case creationFailed

An error that indicates a general failure occurred during image creation.

