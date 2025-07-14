

- UIKit
- NSTextList
-  marker(forItemNumber:) 

Instance Method

# marker(forItemNumber:)

Returns the computed value for a specific ordinal position in the list.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func marker(forItemNumber itemNumber: Int) -> String
```

## Parameters 

`itemNumber`  

The ordinal position in the list whose computed marker value is desired.

## Return Value

The computed maker value for `itemNumber`.

## See Also

### Working with markers

var markerFormat: NSTextList.MarkerFormat

Returns the marker format string used by the receiver.

struct MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

