

- UIKit
- UIImageAsset
-  unregister(imageWith:) 

Instance Method

# unregister(imageWith:)

Unregisters the image with the specified trait collection from the image asset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func unregister(imageWith traitCollection: UITraitCollection)
```

## Parameters 

`traitCollection`  

A trait collection containing the traits for a previously registered image. This method matches only the trait values, so you don’t need to specify the same object you used at registration time.

## Discussion

This method searches for an image whose trait collection matches the one in the `traitCollection` parameter. The traits in both collections must match exactly, and the matching trait collection must be associated with an image that you registered previously.

## See Also

### Registering and unregistering images

func register(UIImage, with: UITraitCollection)

Registers an image with the specified trait collection.

func register(UIImage, with: UIImage.Configuration)

Registers an image with the specified image configuration details.

func unregisterImage(with: UIImage.Configuration)

Unregisters the image with the specified image configuration details from the image asset.

