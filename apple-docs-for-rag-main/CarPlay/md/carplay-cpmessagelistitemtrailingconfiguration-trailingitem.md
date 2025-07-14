

- CarPlay
- CPMessageListItemTrailingConfiguration
-  trailingItem 

Instance Property

# trailingItem

The configuration’s item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var trailingItem: CPMessageTrailingItem { get }
```

## Discussion

Configurations are immutable. To change or remove the item that the message list item’s trailing region shows, create a new configuration and update the list item’s trailingConfiguration property.

## See Also

### Getting the Trailing Item

enum CPMessageTrailingItem

The accessories that a message list item can display in its trailing region.

