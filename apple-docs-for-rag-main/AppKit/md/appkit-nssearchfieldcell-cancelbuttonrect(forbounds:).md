

- AppKit
- NSSearchFieldCell
-  cancelButtonRect(forBounds:) 

Instance Method

# cancelButtonRect(forBounds:)

Modifies the bounding rectangle for the cancel button cell.

macOS

``` source
@MainActor
func cancelButtonRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The current bounding rectangle for the cancel button.

## Return Value

The updated bounding rectangle to use for the cancel button. The default value is the value passed into the `rect` parameter.

## Discussion

Subclasses can override this method to return a new bounding rectangle for the cancel button cell. You might use this method to provide a custom layout for the search field control.

## See Also

### Custom layout

func searchTextRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search-text field cell.

func searchButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search button cell.

