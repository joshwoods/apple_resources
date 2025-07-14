

- UIKit
-  Images and PDF 

API Collection

# Images and PDF

Create and manage images, including those that use bitmap and PDF formats.

## Topics

### Representations

class UIImage

An object that manages image data in your app.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

### Image creation

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

func jpegData(compressionQuality: CGFloat) -> Data?

Returns a data object that contains the image in JPEG format.

func pngData() -> Data?

Returns a data object that contains the specified image in PNG format.

func UIGraphicsBeginImageContext(CGSize)

Creates a bitmap-based graphics context and makes it the current context.

Deprecated

func UIGraphicsGetImageFromCurrentImageContext() -> UIImage?

Returns an image from the contents of the current bitmap-based graphics context.

Deprecated

func UIGraphicsEndImageContext()

Removes the current bitmap-based graphics context from the top of the stack.

Deprecated

### Photo album

func UIImageWriteToSavedPhotosAlbum(UIImage, Any?, Selector?, UnsafeMutableRawPointer?)

Adds the specified image to the user’s Camera Roll album.

func UISaveVideoAtPathToSavedPhotosAlbum(String, Any?, Selector?, UnsafeMutableRawPointer?)

Adds the movie from the specified path to the user’s Camera Roll album.

func UIVideoAtPathIsCompatibleWithSavedPhotosAlbum(String) -> Bool

Returns a Boolean value that indicates whether the specified video is compatible to save to the user’s Camera Roll album.

### PDF creation

func UIGraphicsBeginPDFContextToData(NSMutableData, CGRect, [AnyHashable : Any]?)

Creates a PDF graphics context that targets the specified mutable data object.

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

func UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

func UIGraphicsBeginPDFPage()

Marks the beginning of a new page in a PDF context and configures it using default values.

func UIGraphicsBeginPDFPageWithInfo(CGRect, [AnyHashable : Any]?)

Marks the beginning of a new page in a PDF context and configures it using the specified custom values.

func UIGraphicsGetPDFContextBounds() -> CGRect

Returns the current page bounds.

func UIGraphicsAddPDFContextDestinationAtPoint(String, CGPoint)

Creates a jump destination in the current page.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

func UIGraphicsSetPDFContextURLForRect(URL, CGRect)

Links a rectangular area on the current page to the specified URL.

### PDF screenshots

class UIScreenshotService

An object that coordinates the creation of PDF screenshots of an app’s content.

## See Also

### Graphics, drawing, and printing

Drawing

Configure your app’s drawing environment using colors, renderers, draw paths, strings, and shadows.

Printing

Display the system print panels and manage the printing process.

