

- XCTest
- XCTAttachment
-  init(image:) 

Initializer

# init(image:)

Creates an attachment containing a PNG representation of the provided image.

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
convenience init(image: UIImage)
```

**macOS**

``` source
convenience init(image: NSImage)
```

## Parameters 

`image`  

The image to wrap as an attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of `"public.png"`. Equivalent to calling init(image:quality:) with a `quality` value of XCTAttachment.ImageQuality.original.

## See Also

### Creating Attachments from Images and Screenshots

convenience init(image: UIImage, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided image at the requested image quality.

convenience init(screenshot: XCUIScreenshot)

Creates an attachment containing a PNG representation of the provided screenshot.

convenience init(screenshot: XCUIScreenshot, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided screenshot at the requested image quality.

@MainActor class XCUIScreenshot

A captured image of a screen, app, or UI element state.

enum ImageQuality

Compression quality options for image-based attachments.

