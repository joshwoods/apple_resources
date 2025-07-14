

- AppKit
- NSBrowser
-  setPath(\_:) 

Instance Method

# setPath(\_:)

Sets the path to be displayed by the browser.

macOS

``` source
@MainActor
func setPath(_ path: String) -> Bool
```

## Parameters 

`path`  

The path to display. If `path` is prefixed by the path separator, the path is absolute, containing the full path from the browser’s first column. Otherwise, the path is relative, extending the browser’s current path starting at the last column.

## Return Value

true if the given path is valid; otherwise, false.

## Discussion

While parsing `path`, the browser compares each component with the entries in the current column. If an exact match is found, the matching entry is selected, and the next component is compared to the next column’s entries. If no match is found for a component, the method exits and returns false; the final path is set to the valid portion of `path`. If each component of `path` specifies a valid branch or leaf in the browser’s hierarchy, the method returns true.

## See Also

### Managing the Path

func path() -> String

Returns a string representing the browser’s current path.

func path(toColumn: Int) -> String

Returns a string representing the path from the first column up to, but not including, the column at the given index.

var pathSeparator: String

The path separator.

