

- CarPlay
- CPMessageListItemLeadingConfiguration
-  init(leadingItem:leadingImage:unread:) 

Initializer

# init(leadingItem:leadingImage:unread:)

Creates a leading configuration that contains an item and an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    leadingItem: CPMessageLeadingItem,
    leadingImage: UIImage?,
    unread: Bool
)
```

## Parameters 

`leadingItem`  

The item to show in the leading region of the message list item. See CPMessageLeadingItem for the available options.

`leadingImage`  

The image to show in the leading region of the message list item.

`unread`  

If true, the message list item displays an indicator that shows the message is in an unread state.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. Make sure that the image isn’t larger than CPMaximumMessageItemImageSize.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a Configuration

let CPMaximumMessageItemImageSize: CGSize

The maximum size of a message list item’s image.

