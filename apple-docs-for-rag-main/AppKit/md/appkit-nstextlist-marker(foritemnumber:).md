

- AppKit
- NSTextList
-  marker(forItemNumber:) 

Instance Method

# marker(forItemNumber:)

Returns the computed value for a specific ordinal position in the list.

macOS 10.0+

``` source
func marker(forItemNumber itemNumber: Int) -> String
```

## Parameters 

`itemNumber`  

The ordinal position in the list whose computed marker value is desired.

## Return Value

The computed maker value for `itemNum`.

## See Also

### Working with markers

var markerFormat: NSTextList.MarkerFormat

Returns the marker format string used by the receiver.

struct MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

