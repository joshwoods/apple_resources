

- UIKit
- UIImageAsset
-  image(with:) 

Instance Method

# image(with:)

Retrieves the variant of the image that best matches the specified image configuration details.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func image(with configuration: UIImage.Configuration) -> UIImage
```

## Parameters 

`configuration`  

The configuration details to use when determining which image to return.

## Return Value

The image object for the specified configuration.

## Discussion

If this method can’t locate an image that matches the specified image configuration precisely, it returns the best match available.

## See Also

### Retrieving an image from an image asset

func image(with: UITraitCollection) -> UIImage

Retrieves the variant of the image that best matches the specified trait collection.

