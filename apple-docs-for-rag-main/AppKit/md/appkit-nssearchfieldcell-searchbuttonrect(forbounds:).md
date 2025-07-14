

- AppKit
- NSSearchFieldCell
-  searchButtonRect(forBounds:) 

Instance Method

# searchButtonRect(forBounds:)

Modifies the bounding rectangle for the search button cell.

macOS

``` source
@MainActor
func searchButtonRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The current bounding rectangle for the search button.

## Return Value

The updated bounding rectangle to use for the search button. The default value is the value passed into the `rect` parameter.

## Discussion

Subclasses can override this method to return a new bounding rectangle for the search button cell. You might use this method to provide a custom layout for the search field control.

## See Also

### Custom layout

func searchTextRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search-text field cell.

func cancelButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the cancel button cell.

