

- CarPlay
- CPListItem
-  init(text:detailText:) 

Initializer

# init(text:detailText:)

Creates a list item with primary and secondary text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    text: String?,
    detailText: String?
)
```

## Parameters 

`text`  

The primary text to show in the list item cell.

`detailText`  

Additional text to display below the primary text in the list item cell.

## Return Value

A newly initialized list item.

## See Also

### Creating a List Item

init(text: String?, detailText: String?, image: UIImage?)

Creates a list item with primary text, secondary text, and an image.

init(text: String?, detailText: String?, image: UIImage?, accessoryImage: UIImage?, accessoryType: CPListItemAccessoryType)

Creates a list item that displays an accessory beside its content.

