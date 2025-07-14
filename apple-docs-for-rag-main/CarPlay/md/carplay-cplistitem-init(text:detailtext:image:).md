

- CarPlay
- CPListItem
-  init(text:detailText:image:) 

Initializer

# init(text:detailText:image:)

Creates a list item with primary text, secondary text, and an image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    text: String?,
    detailText: String?,
    image: UIImage?
)
```

## Parameters 

`text`  

The primary text to show in the list item cell.

`detailText`  

Additional text to display below the primary text in the list item cell.

`image`  

The image to display on the leading edge of the list item cell. If the image is larger than `CPMaximumListItemImageSize`, the list item scales down the image to maximum size. If you provide an animated image, the list item uses the first image in the animation sequence.

## Return Value

A newly initialized list item.

## See Also

### Creating a List Item

init(text: String?, detailText: String?)

Creates a list item with primary and secondary text.

init(text: String?, detailText: String?, image: UIImage?, accessoryImage: UIImage?, accessoryType: CPListItemAccessoryType)

Creates a list item that displays an accessory beside its content.

