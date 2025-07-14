

- CarPlay
- CPListItem
-  init(text:detailText:image:accessoryImage:accessoryType:) 

Initializer

# init(text:detailText:image:accessoryImage:accessoryType:)

Creates a list item that displays an accessory beside its content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    text: String?,
    detailText: String?,
    image: UIImage?,
    accessoryImage: UIImage?,
    accessoryType: CPListItemAccessoryType
)
```

## Parameters 

`text`  

The list item’s primary text.

`detailText`  

The list item’s secondary text.

`image`  

The image that the list item displays in its leading region.

`accessoryImage`  

The image that the list item displays in its trailing region.

`accessoryType`  

The accessory that the list item displays in its trailing region.

## Discussion

If you specify an image, CarPlay sets `accessoryType` to CPListItemAccessoryType.none.

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size for a list item’s image and accessory image.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a List Item

init(text: String?, detailText: String?)

Creates a list item with primary and secondary text.

init(text: String?, detailText: String?, image: UIImage?)

Creates a list item with primary text, secondary text, and an image.

