

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldExpandItem:) 

Instance Method

# outlineView(\_:shouldExpandItem:)

Returns a Boolean value that indicates whether the outline view should expand a given item.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldExpandItem item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

The item that should expand.

## Return Value

true to permit `outlineView` to expand `item`, false to deny permission.

## Discussion

The delegate can implement this method to disallow expanding of specific items.

## See Also

### Related Documentation

Outline View Programming Topics

Drag and Drop Programming Topics

### Expanding and Collapsing the Outline

func outlineView(NSOutlineView, shouldCollapseItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should collapse a given item.

