

- XCTest
- XCTAttachment
-  XCTAttachment.ImageQuality 

Enumeration

# XCTAttachment.ImageQuality

Compression quality options for image-based attachments.

``` source
enum ImageQuality
```

## Topics

### Quality Settings

case original

Original image quality, represented as a lossless PNG image.

case medium

Medium image quality, represented as a high quality lossy JPEG image.

case low

Low image quality, represented as a highly compressed lossy JPEG image.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Attachments from Images and Screenshots

convenience init(image: UIImage)

Creates an attachment containing a PNG representation of the provided image.

convenience init(image: UIImage, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided image at the requested image quality.

convenience init(screenshot: XCUIScreenshot)

Creates an attachment containing a PNG representation of the provided screenshot.

convenience init(screenshot: XCUIScreenshot, quality: XCTAttachment.ImageQuality)

Creates an attachment containing a representation of the provided screenshot at the requested image quality.

@MainActor class XCUIScreenshot

A captured image of a screen, app, or UI element state.

