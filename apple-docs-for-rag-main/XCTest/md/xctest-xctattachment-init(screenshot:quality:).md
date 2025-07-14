

- XCTest
- XCTAttachment
-  init(screenshot:quality:) 

Initializer

# init(screenshot:quality:)

Creates an attachment containing a representation of the provided screenshot at the requested image quality.

``` source
convenience init(
    screenshot: XCUIScreenshot,
    quality: XCTAttachment.ImageQuality
)
```

## Parameters 

`screenshot`  

The screenshot to wrap as an attachment.

`quality`  

The quality setting to use when storing the screenshot in the attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of `"public.png"` when `quality` is XCTAttachment.ImageQuality.original, and a uniformTypeIdentifier of `"public.jpeg"` when `quality` is XCTAttachment.ImageQuality.medium or XCTAttachment.ImageQuality.low.

## See Also

### Creating Attachments from Images and Screenshots

convenience init(image: UIImage)

Creates an attachment containing a PNG representation of the provided image.

convenience init(image: UIImage, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided image at the requested image quality.

convenience init(screenshot: XCUIScreenshot)

Creates an attachment containing a PNG representation of the provided screenshot.

@MainActor class XCUIScreenshot

A captured image of a screen, app, or UI element state.

enum ImageQuality

Compression quality options for image-based attachments.

