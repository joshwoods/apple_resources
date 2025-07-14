

- UIKit
-  UIImageWriteToSavedPhotosAlbum(\_:\_:\_:\_:) 

Function

# UIImageWriteToSavedPhotosAlbum(\_:\_:\_:\_:)

Adds the specified image to the user’s Camera Roll album.

iOSiPadOSMac CatalystvisionOS

``` source
func UIImageWriteToSavedPhotosAlbum(
    _ image: UIImage,
    _ completionTarget: Any?,
    _ completionSelector: Selector?,
    _ contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`image`  

The image to write to the Camera Roll album.

`completionTarget`  

Optionally, the object whose selector should be called after the image has been written to the Camera Roll album.

`completionSelector`  

The method selector of the `completionTarget` object to call. This optional method should conform to the following signature:

```
- (void)image:(UIImage *)image
    didFinishSavingWithError:(NSError *)error
                 contextInfo:(void *)contextInfo;
```

`contextInfo`  

An optional pointer to any context-specific data that you want passed to the completion selector.

## Discussion

When used with an image picker controller, you would typically call this function within your imagePickerController(_:didFinishPickingMediaWithInfo:) delegate method implementation.

The use of the `completionTarget`, `completionSelector`, and `contextInfo` parameters is optional and necessary only if you want to be notified asynchronously when the function finishes writing the image to the user’s Camera Roll or Saved Photos album. If you do not want to be notified, pass `nil` for these parameters.

When used on an iOS device without a camera, this method adds the image to the Saved Photos album rather than to the Camera Roll album.

## See Also

### Photo album

func UISaveVideoAtPathToSavedPhotosAlbum(String, Any?, Selector?, UnsafeMutableRawPointer?)

Adds the movie from the specified path to the user’s Camera Roll album.

func UIVideoAtPathIsCompatibleWithSavedPhotosAlbum(String) -> Bool

Returns a Boolean value that indicates whether the specified video is compatible to save to the user’s Camera Roll album.

