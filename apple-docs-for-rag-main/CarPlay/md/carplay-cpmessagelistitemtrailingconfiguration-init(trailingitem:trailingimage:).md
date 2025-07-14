

- CarPlay
- CPMessageListItemTrailingConfiguration
-  init(trailingItem:trailingImage:) 

Initializer

# init(trailingItem:trailingImage:)

Creates a trailing configuration that contains an item and an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    trailingItem: CPMessageTrailingItem,
    trailingImage: UIImage?
)
```

## Parameters 

`trailingItem`  

The item to show in the trailing region of the message list item. See CPMessageTrailingItem for the available options.

`trailingImage`  

The image to show in the trailing region of the message list item.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. Make sure that the image isn’t larger than CPMaximumMessageItemImageSize.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a Configuration

let CPMaximumMessageItemImageSize: CGSize

The maximum size of a message list item’s image.

