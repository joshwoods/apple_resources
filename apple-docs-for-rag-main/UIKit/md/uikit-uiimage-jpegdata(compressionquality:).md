

- UIKit
- UIImage
-  jpegData(compressionQuality:) 

Instance Method

# jpegData(compressionQuality:)

Returns a data object that contains the image in JPEG format.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func jpegData(compressionQuality: CGFloat) -> Data?
```

## Parameters 

`compressionQuality`  

The quality of the resulting JPEG image, expressed as a value from `0.0` to `1.0`. The value `0.0` represents the maximum compression (or lowest quality) while the value `1.0` represents the least compression (or best quality).

## Return Value

A data object containing the JPEG data, or `nil` if there’s a problem generating the data. This function may return `nil` if the image has no data or if the underlying `CGImageRef` contains data in an unsupported bitmap format.

## Discussion

If the image object’s underlying image data has been purged, calling this function forces that data to be reloaded into memory.

## See Also

### Image creation

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

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

