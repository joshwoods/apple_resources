

- UIKit
-  UIGraphicsEndImageContext() 

Function

# UIGraphicsEndImageContext()

Removes the current bitmap-based graphics context from the top of the stack.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
func UIGraphicsEndImageContext()
```

## Discussion

You use this function to clean up the drawing environment put in place by the UIGraphicsBeginImageContext(_:) function and to remove the corresponding bitmap-based graphics context from the top of the stack. If the current context was not created using the UIGraphicsBeginImageContext(_:) function, this function does nothing.

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

func UIGraphicsGetImageFromCurrentImageContext() -> UIImage?

Returns an image from the contents of the current bitmap-based graphics context.

Deprecated

