

- UIKit
-  UIGraphicsGetImageFromCurrentImageContext() 

Function

# UIGraphicsGetImageFromCurrentImageContext()

Returns an image from the contents of the current bitmap-based graphics context.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
func UIGraphicsGetImageFromCurrentImageContext() -> UIImage?
```

## Return Value

A image object containing the contents of the current bitmap graphics context.

## Discussion

You should call this function only when a bitmap-based graphics context is the current graphics context. If the current context is `nil` or was not created by a call to UIGraphicsBeginImageContext(_:), this function returns `nil`.

This function may be called from any thread of your app.

## See Also

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

func UIGraphicsEndImageContext()

Removes the current bitmap-based graphics context from the top of the stack.

Deprecated

