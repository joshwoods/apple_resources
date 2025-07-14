

- UIKit
- NSTextList
-  markerFormat 

Instance Property

# markerFormat

Returns the marker format string used by the receiver.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var markerFormat: NSTextList.MarkerFormat { get }
```

## Return Value

The marker format string used by the receiver.

## See Also

### Related Documentation

convenience init(markerFormat: NSTextList.MarkerFormat, options: Int)

Returns an initialized text list.

### Working with markers

struct MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

func marker(forItemNumber: Int) -> String

Returns the computed value for a specific ordinal position in the list.

