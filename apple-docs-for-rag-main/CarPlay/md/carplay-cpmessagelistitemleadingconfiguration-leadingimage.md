

- CarPlay
- CPMessageListItemLeadingConfiguration
-  leadingImage 

Instance Property

# leadingImage

The configuration’s image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var leadingImage: UIImage? { get }
```

## Discussion

Configurations are immutable. To change or remove the image that the message list item’s leading region shows, create a new configuration and update the list item’s leadingConfiguration property.

A configuration’s image can’t be larger than CPMaximumMessageItemImageSize. If you use an animated image, this property returns the first image in the animation sequence.

## See Also

### Getting the Configuration’s State

var isUnread: Bool

A Boolean value that determines whether the message list item displays an unread indicator.

