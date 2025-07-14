

- XCTest
- XCTAttachment
-  init(image:quality:) 

Initializer

# init(image:quality:)

Creates an attachment containing a representation of the provided image at the requested image quality.

**macOS**

``` source
convenience init(
    image: NSImage,
    quality: XCTAttachment.ImageQuality
)
```

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
convenience init(
    image: UIImage,
    quality: XCTAttachment.ImageQuality
)
```

## Parameters 

`image`  

The image to wrap as an attachment.

`quality`  

The quality setting to use when storing the image in the attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of `"public.png"` when `quality` is XCTAttachment.ImageQuality.original, and a uniformTypeIdentifier of `"public.jpeg"` when `quality` is XCTAttachment.ImageQuality.medium or XCTAttachment.ImageQuality.low.

## See Also

### Creating Attachments from Images and Screenshots

convenience init(image: UIImage)

Creates an attachment containing a PNG representation of the provided image.

convenience init(screenshot: XCUIScreenshot)

Creates an attachment containing a PNG representation of the provided screenshot.

convenience init(screenshot: XCUIScreenshot, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided screenshot at the requested image quality.

@MainActor class XCUIScreenshot

A captured image of a screen, app, or UI element state.

enum ImageQuality

Compression quality options for image-based attachments.

