

- AppKit
- NSBrowser
-  pathSeparator 

Instance Property

# pathSeparator

The path separator.

macOS

``` source
@MainActor
var pathSeparator: String { get set }
```

## Discussion

The default value of this property is `/`.

## See Also

### Managing the Path

func path() -> String

Returns a string representing the browser’s current path.

func setPath(String) -> Bool

Sets the path to be displayed by the browser.

func path(toColumn: Int) -> String

Returns a string representing the path from the first column up to, but not including, the column at the given index.

