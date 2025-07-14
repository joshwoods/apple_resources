

- UIKit
- UIImage
-  prepareForDisplay(completionHandler:) 

Instance Method

# prepareForDisplay(completionHandler:)

Decodes an image asynchronously and provides a new one for display in views and animations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func prepareForDisplay(completionHandler: @escaping (UIImage?) -> Void)
```

``` source
func byPreparingForDisplay() async -> UIImage?
```

## Parameters 

`completionHandler`  

The closure to call when the function finishes preparing the image.

This completion handler takes one parameter:

`image`  
A new version of the image object for display. If the system can’t decode the image, the parameter value is `nil.`

## Discussion

The Animation Hitches instrument measures system performance for multiple stages of preparing views for display. It can show you the exact cause of an animation hitch, which appears to the user as an interruption or jump in an animation that should be smooth. If Animation Hitches indicates that decoding an image takes too long and causes hitches, use this method to move the decoding work to the background.

This method creates a new image object and passes it to the completion handler. The new image is ready for efficient display by an image view. Assign the image this method creates to the image property of an image view. If UIImageView can render the image without decoding, this method passes the completion handler a valid image without further processing. If the system can’t decode the image, such as an image created from a CIImage, the method passes `nil` to the completion handler`.`

UIKit doesn’t associate the prepared image with the original, or with any related variants from an asset catalog. If your app environment dynamically changes display traits, listen for changes in the trait environment and prepare new images when the environment changes.

```
func collectionView(_ collectionView: UICollectionView, prefetchItemsAt indexPaths: [IndexPath]) {
    for path in indexPaths {
        let item = models[path.item]
        if preparedImageCache.object(forKey: item.id) == nil {
            item.loadAsset()
            item.image.prepareForDisplay { [weak preparedImageCache] preparedImage in
                if let preparedImage = preparedImage {
                    preparedImageCache?.setObject(preparedImage, forKey: item.id)
                }
            }
        }
    }
}
```

## See Also

### Loading images for display

func preparingForDisplay() -> UIImage?

Decodes an image synchronously and provides a new one for display in views and animations.

func preparingThumbnail(of: CGSize) -> UIImage?

Returns a new thumbnail image at the specified size.

func prepareThumbnail(of: CGSize, completionHandler: (UIImage?) -> Void)

Creates a thumbnail image at the specified size asynchronously on a background thread.

