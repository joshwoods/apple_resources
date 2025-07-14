

- XCTest
-  XCTAttachment 

Class

# XCTAttachment

Data from a test method’s execution, such as a file, image, screenshot, data blob, or ZIP file.

``` source
class XCTAttachment
```

## Mentioned in 

Adding Attachments to Tests, Activities, and Issues

## Topics

### Creating Attachments from Data

convenience init(data: Data)

Creates an attachment containing the provided data payload.

convenience init(data: Data, uniformTypeIdentifier: String)

Creates an attachment containing the provided data payload, with a custom UTI.

init(uniformTypeIdentifier: String?, name: String?, payload: Data?, userInfo: [AnyHashable : Any]?)

Creates an attachment containing the provided data payload, optionally with a custom UTI, name, and user-provided metadata dictionary.

### Creating Attachments from Files and Folders

convenience init(contentsOfFileAtURL: URL)

Creates an attachment from the contents of an existing file on disk.

Deprecated

convenience init(contentsOfFileAtURL: URL, uniformTypeIdentifier: String)

Creates an attachment from the contents of an existing file on disk, with a custom UTI.

Deprecated

convenience init(compressedContentsOfDirectoryAtURL: URL)

Creates an attachment containing a zipped archive of an existing directory on disk.

Deprecated

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

enum ImageQuality

Compression quality options for image-based attachments.

### Creating Attachments from Objects

convenience init(plistObject: Any)

Creates an attachment from an object that can be represented in an XML property list.

convenience init(archivableObject: any NSSecureCoding)

Creates an attachment from an object that conforms to `NSSecureCoding`.

convenience init(archivableObject: any NSSecureCoding, uniformTypeIdentifier: String)

Creates an attachment from an object that conforms to `NSSecureCoding`, with a custom UTI.

### Creating Attachments from Strings

convenience init(string: String)

Creates an attachment containing the provided string.

### Setting an Attachment’s Lifetime

var lifetime: XCTAttachment.Lifetime

Indicates whether the attachment is kept or discarded when its associated test passes.

enum Lifetime

The possible lifetime values for a test attachment.

### Attachment Metadata

var name: String?

The attachment’s name, or `nil` if the attachment is unnamed.

var uniformTypeIdentifier: String

The Uniform Type Identifier (UTI) of the data represented by the attachment.

var userInfo: [AnyHashable : Any]?

User-provided metadata associated with the attachment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Attachments

Adding Attachments to Tests, Activities, and Issues

Use attachments to store a test’s output data for later analysis.

