

- AppKit
- NSMenuItemBadge
-  newItems(count:) 

Type Method

# newItems(count:)

Creates a new item-style badge with an integer count and a predefined label that represents the number of new items.

macOS 14.0+

``` source
class func newItems(count itemCount: Int) -> Self
```

## Parameters 

`itemCount`  

The badge count.

## Return Value

Returns a new badge item of type NSMenuItemBadge.BadgeType.newItems.

## See Also

### Creating badges of a specific type

class func alerts(count: Int) -> Self

Creates an alert-style badge with an integer count and a predefined label that represents the number of alerts.

class func updates(count: Int) -> Self

Creates an update-style badge with an integer count and a predefined label that represents the number of available updates.

enum BadgeType

Constants that define types of badges for display.

