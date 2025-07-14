

- CarPlay
- CPListItem
-  init(text:detailText:image:showsDisclosureIndicator:) Deprecated

Initializer

# init(text:detailText:image:showsDisclosureIndicator:)

Creates a list item with primary text, secondary text, an image, and a disclosure indicator.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
init(
    text: String?,
    detailText: String?,
    image: UIImage?,
    showsDisclosureIndicator: Bool
)
```

Deprecated

Use init(text:detailText:image:accessoryImage:accessoryType:) instead.

## Parameters 

`text`  

The primary text to show in the list item cell.

`detailText`  

Additional text to display below the primary text in the list item cell.

`image`  

The image to display on the leading edge of the list item cell. If the image is larger than `CPMaximumListItemImageSize`, the list item scales down the image to maximum size. If you provide an animated image, the list item uses the first image in the animation sequence.

`showsDisclosureIndicator`  

A Boolean value that indicates whether the list item cell displays a disclosure indicator. Set to true to display the indicator on the trailing edge of the list item cell.

## Return Value

A newly initialized list item.

