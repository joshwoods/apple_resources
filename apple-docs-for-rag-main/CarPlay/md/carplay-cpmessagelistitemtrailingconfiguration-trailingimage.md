

- CarPlay
- CPMessageListItemTrailingConfiguration
-  trailingImage 

Instance Property

# trailingImage

The configuration’s image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var trailingImage: UIImage? { get }
```

## Discussion

Configurations are immutable. To change or remove the image that the message list item’s trailing region shows, create a new configuration and update the list item’s trailingConfiguration property.

A configuration’s image can’t be larger than CPMaximumMessageItemImageSize. If you use an animated image, this property returns the first image in the animation sequence.

