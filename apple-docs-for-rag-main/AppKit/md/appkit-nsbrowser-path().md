

- AppKit
- NSBrowser
-  path() 

Instance Method

# path()

Returns a string representing the browser’s current path.

macOS

``` source
@MainActor
func path() -> String
```

## Return Value

The path representing the current selection. The components of this path are separated with the string returned by pathSeparator.

## Discussion

Invoking this method is equivalent to invoking path(toColumn:) for all columns.

## See Also

### Managing the Path

func setPath(String) -> Bool

Sets the path to be displayed by the browser.

func path(toColumn: Int) -> String

Returns a string representing the path from the first column up to, but not including, the column at the given index.

var pathSeparator: String

The path separator.

