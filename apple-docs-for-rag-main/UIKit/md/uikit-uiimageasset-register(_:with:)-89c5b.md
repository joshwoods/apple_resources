

- UIKit
- UIImageAsset
-  register(\_:with:) 

Instance Method

# register(\_:with:)

Registers an image with the specified image configuration details.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func register(
    _ image: UIImage,
    with configuration: UIImage.Configuration
)
```

## Parameters 

`image`  

The image you want to register with the image asset.

`configuration`  

The image configuration details to associate with `image`.

## Discussion

Each image in an image asset must have a unique configuration. If the asset already contains a registered image with the equivalent configuration, it replaces that image with the one in the `image` parameter.

Important

The trait collection in `configuration` must always contain an explicit value in its displayScale property. You may experience unexpected results from image(with:) if the trait collection doesn’t explicitly define the desired scale.

## See Also

### Registering and unregistering images

func register(UIImage, with: UITraitCollection)

Registers an image with the specified trait collection.

func unregister(imageWith: UITraitCollection)

Unregisters the image with the specified trait collection from the image asset.

func unregisterImage(with: UIImage.Configuration)

Unregisters the image with the specified image configuration details from the image asset.

