

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldCollapseItem:) 

Instance Method

# outlineView(\_:shouldCollapseItem:)

Returns a Boolean value that indicates whether the outline view should collapse a given item.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldCollapseItem item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

The item that should collapse.

## Return Value

true to permit `outlineView` to collapse `item`, false to deny permission.

## Discussion

The delegate can implement this method to disallow collapsing of specific items. For example, if the first row of your outline view should not be collapsed, your delegate method could contain this line of code:

```
return [outlineView rowForItem:item]!=0;
```

## See Also

### Expanding and Collapsing the Outline

func outlineView(NSOutlineView, shouldExpandItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should expand a given item.

