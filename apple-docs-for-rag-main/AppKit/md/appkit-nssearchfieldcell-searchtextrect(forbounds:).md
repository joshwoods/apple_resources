

- AppKit
- NSSearchFieldCell
-  searchTextRect(forBounds:) 

Instance Method

# searchTextRect(forBounds:)

Modifies the bounding rectangle for the search-text field cell.

macOS

``` source
@MainActor
func searchTextRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The current bounding rectangle for the search text field.

## Return Value

The updated bounding rectangle to use for the search text field. The default value is the value passed into the `rect` parameter.

## Discussion

Subclasses can override this method to return a new bounding rectangle for the text-field cell object. You might use this method to provide a custom layout for the search field control.

## See Also

### Custom layout

func searchButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the search button cell.

func cancelButtonRect(forBounds: NSRect) -> NSRect

Modifies the bounding rectangle for the cancel button cell.

