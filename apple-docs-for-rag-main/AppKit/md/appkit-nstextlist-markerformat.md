

- AppKit
- NSTextList
-  markerFormat 

Instance Property

# markerFormat

Returns the marker format string used by the receiver.

macOS 10.0+

``` source
var markerFormat: NSTextList.MarkerFormat { get }
```

## Return Value

The marker format string used by the receiver.

## See Also

### Working with markers

struct MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

func marker(forItemNumber: Int) -> String

Returns the computed value for a specific ordinal position in the list.

