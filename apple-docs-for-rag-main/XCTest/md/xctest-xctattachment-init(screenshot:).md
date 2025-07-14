

- XCTest
- XCTAttachment
-  init(screenshot:) 

Initializer

# init(screenshot:)

Creates an attachment containing a PNG representation of the provided screenshot.

``` source
convenience init(screenshot: XCUIScreenshot)
```

## Parameters 

`screenshot`  

The screenshot to wrap as an attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of `"public.png"`. Equivalent to calling init(screenshot:quality:) with a `quality` value of XCTAttachment.ImageQuality.original.

## See Also

### Creating Attachments from Images and Screenshots

convenience init(image: UIImage)

Creates an attachment containing a PNG representation of the provided image.

convenience init(image: UIImage, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided image at the requested image quality.

convenience init(screenshot: XCUIScreenshot, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided screenshot at the requested image quality.

@MainActor class XCUIScreenshot

A captured image of a screen, app, or UI element state.

enum ImageQuality

Compression quality options for image-based attachments.

