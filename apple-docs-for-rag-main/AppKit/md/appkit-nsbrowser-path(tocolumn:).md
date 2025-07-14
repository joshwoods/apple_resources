

- AppKit
- NSBrowser
-  path(toColumn:) 

Instance Method

# path(toColumn:)

Returns a string representing the path from the first column up to, but not including, the column at the given index.

macOS

``` source
@MainActor
func path(toColumn column: Int) -> String
```

## Parameters 

`column`  

The index of the column at which the path stops.

## Return Value

The path of the current selection up to, but not including, the specified column. The components of this path are separated with the string returned by pathSeparator.

## See Also

### Managing the Path

func path() -> String

Returns a string representing the browser’s current path.

func setPath(String) -> Bool

Sets the path to be displayed by the browser.

var pathSeparator: String

The path separator.

