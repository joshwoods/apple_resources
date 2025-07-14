

- UIKit
-  UIGraphicsBeginImageContext(\_:) 

Function

# UIGraphicsBeginImageContext(\_:)

Creates a bitmap-based graphics context and makes it the current context.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
func UIGraphicsBeginImageContext(_ size: CGSize)
```

## Parameters 

`size`  

The size of the new bitmap context. This represents the size of the image returned by the UIGraphicsGetImageFromCurrentImageContext() function.

## Discussion

This function is equivalent to calling the UIGraphicsBeginImageContextWithOptions(_:_:_:) function with the opaque parameter set to false and a scale factor of `1.0`.

This function may be called from any thread of your app.

## See Also

### Image creation

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

func jpegData(compressionQuality: CGFloat) -> Data?

Returns a data object that contains the image in JPEG format.

func pngData() -> Data?

Returns a data object that contains the specified image in PNG format.

func UIGraphicsGetImageFromCurrentImageContext() -> UIImage?

Returns an image from the contents of the current bitmap-based graphics context.

Deprecated

func UIGraphicsEndImageContext()

Removes the current bitmap-based graphics context from the top of the stack.

Deprecated

