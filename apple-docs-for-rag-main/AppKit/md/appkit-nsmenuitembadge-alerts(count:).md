

- AppKit
- NSMenuItemBadge
-  alerts(count:) 

Type Method

# alerts(count:)

Creates an alert-style badge with an integer count and a predefined label that represents the number of alerts.

macOS 14.0+

``` source
class func alerts(count itemCount: Int) -> Self
```

## Parameters 

`itemCount`  

The badge count.

## Return Value

Returns a new badge item of type NSMenuItemBadge.BadgeType.alerts.

## See Also

### Creating badges of a specific type

class func newItems(count: Int) -> Self

Creates a new item-style badge with an integer count and a predefined label that represents the number of new items.

class func updates(count: Int) -> Self

Creates an update-style badge with an integer count and a predefined label that represents the number of available updates.

enum BadgeType

Constants that define types of badges for display.

