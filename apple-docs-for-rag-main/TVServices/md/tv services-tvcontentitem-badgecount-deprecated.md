

- TV Services
- TVContentItem
-  badgeCount Deprecated

Instance Property

# badgeCount

A badging integer for this item.

tvOS 9.0–13.0Deprecated

``` source
@NSCopying
var badgeCount: NSNumber? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

The display-badge number is interpreted as a positive integer. Not all UI elements that use content items display badges.

## See Also

### Inspecting the General Display Properties

var title: String?

The localized string title of the item.

Deprecated

var topShelfItems: [TVContentItem]?

An array of content items that are the items of a section.

Deprecated

