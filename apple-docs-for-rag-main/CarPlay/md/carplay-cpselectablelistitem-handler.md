

- CarPlay
- CPSelectableListItem
-  handler 

Instance Property

# handler

An optional closure that CarPlay invokes when the user selects the list item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var handler: ((any CPSelectableListItem, @escaping () -> Void) -> Void)? { get set }
```

**Required**

