

- UIKit
- UIImageAsset
-  image(with:) 

Instance Method

# image(with:)

Retrieves the variant of the image that best matches the specified trait collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func image(with traitCollection: UITraitCollection) -> UIImage
```

## Parameters 

`traitCollection`  

The trait collection to use when determining which image to return.

## Return Value

The found image.

## Discussion

If this method can’t locate an image that matches the specified trait collection precisely, it returns the best match available.

## See Also

### Retrieving an image from an image asset

func image(with: UIImage.Configuration) -> UIImage

Retrieves the variant of the image that best matches the specified image configuration details.

