

- CarPlay
-  CPMaximumMessageItemImageSize 

Global Variable

# CPMaximumMessageItemImageSize

The maximum size of a message list item’s image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
let CPMaximumMessageItemImageSize: CGSize
```

## Discussion

At runtime, use this value to determine the maximum size of an image that a message list item can display in its leading and trailing regions.

## See Also

### Creating a Configuration

init(leadingItem: CPMessageLeadingItem, leadingImage: UIImage?, unread: Bool)

Creates a leading configuration that contains an item and an image.

