

- UIKit
- UIImageAsset
-  unregisterImage(with:) 

Instance Method

# unregisterImage(with:)

Unregisters the image with the specified image configuration details from the image asset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func unregisterImage(with configuration: UIImage.Configuration)
```

## Parameters 

`configuration`  

An object containing the image configuration details for a previously registered image. This method matches only the contents of the object, so you don’t need to specify the same object you used at registration time.

## Discussion

This method searches for an image whose configuration details match the information in the `configuration` parameter. The configuration details must match exactly, and must be associated with an image that you registered previously.

## See Also

### Registering and unregistering images

func register(UIImage, with: UITraitCollection)

Registers an image with the specified trait collection.

func register(UIImage, with: UIImage.Configuration)

Registers an image with the specified image configuration details.

func unregister(imageWith: UITraitCollection)

Unregisters the image with the specified trait collection from the image asset.

