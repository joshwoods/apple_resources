

- CarPlay
- CPListItem
-  setAccessoryImage(\_:) 

Instance Method

# setAccessoryImage(\_:)

Updates the list item’s accessory image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func setAccessoryImage(_ accessoryImage: UIImage?)
```

## Parameters 

`accessoryImage`  

The image to display in the item’s trailing region.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size for a list item’s accessory image.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

CarPlay sets the `accessoryType` property’s value to CPListItemAccessoryType.none when you call this method.

## See Also

### Managing Accessories

var accessoryType: CPListItemAccessoryType

The accessory that the list item displays in its trailing region.

enum CPListItemAccessoryType

The accessory types that a list item can display.

var accessoryImage: UIImage?

The image that the list item displays in its trailing region.

