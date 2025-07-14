

- CarPlay
- CPMessageListItemLeadingConfiguration
-  isUnread 

Instance Property

# isUnread

A Boolean value that determines whether the message list item displays an unread indicator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isUnread: Bool { get }
```

## Discussion

Configurations are immutable. To toggle the message list item’s unread indicator, create a new configuration and update the list item’s leadingConfiguration property.

## See Also

### Getting the Configuration’s State

var leadingImage: UIImage?

The configuration’s image.

