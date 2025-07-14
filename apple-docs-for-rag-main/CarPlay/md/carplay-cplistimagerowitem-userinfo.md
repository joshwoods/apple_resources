

- CarPlay
- CPListImageRowItem
-  userInfo 

Instance Property

# userInfo

An opaque value for the list item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var userInfo: Any? { get set }
```

## Discussion

Use this property to attach a value that provides additional context to the list item. For example, you can attach a model object and reference it in the list item’s handler or listImageRowHandler when processing either selection.

