

- CarPlay
- CPListItem
-  userInfo 

Instance Property

# userInfo

An opaque value for the list item.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var userInfo: Any? { get set }
```

## Discussion

Use this property to attach a value that provides additional context to the list item. For example, you can attach a model object and reference it in the list item’s handler when processing the selection.

## See Also

### Managing Configuration

var isEnabled: Bool

A Boolean value that indicates if the item is enabled.

var handler: ((any CPSelectableListItem, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects the list item.

