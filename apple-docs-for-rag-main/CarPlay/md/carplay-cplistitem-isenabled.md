

- CarPlay
- CPListItem
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates if the item is enabled.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

The default value is true.

## See Also

### Managing Configuration

var handler: ((any CPSelectableListItem, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects the list item.

var userInfo: Any?

An opaque value for the list item.

