

- TV Services
- TVContentItem
-  topShelfItems Deprecated

Instance Property

# topShelfItems

An array of content items that are the items of a section.

tvOS 9.0–13.0Deprecated

``` source
var topShelfItems: [TVContentItem]? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

If this property is non-`nil`, the content item represents a section item in a sectioned Top Shelf style. For more information, see TVTopShelfContentStyle. The title property must also be set to a non-`nil` string.

## See Also

### Inspecting the General Display Properties

var badgeCount: NSNumber?

A badging integer for this item.

Deprecated

var title: String?

The localized string title of the item.

Deprecated

