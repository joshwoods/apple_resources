

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:isGroupItem:) 

Instance Method

# outlineView(\_:isGroupItem:)

Returns a Boolean that indicates whether a given row should be drawn in the “group row” style.

macOS 10.5+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    isGroupItem item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

An item in the outline view.

## Return Value

true to indicate a particular row should have the “group row” style drawn for that row, otherwise false.

## Discussion

If the cell in that row is an instance of `NSTextFieldCell` and contains only a string value, the “group row” style attributes are automatically applied for that cell.

