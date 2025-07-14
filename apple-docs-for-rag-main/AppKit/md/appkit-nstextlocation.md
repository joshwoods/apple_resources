

- AppKit
-  NSTextLocation 

Protocol

# NSTextLocation

An interface you implement that represents an abstract location inside your document’s content.

macOS 12.0+

``` source
protocol NSTextLocation : NSObjectProtocol
```

## Topics

### Comparing text locations

func compare(any NSTextLocation) -> ComparisonResult

Compares and returns the logical ordering to location.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Location and selection

class NSTextRange

A class that represents a contiguous range between two locations inside document contents.

class NSTextSelection

A class that represents a single logical selection context that corresponds to an insertion point.

class NSTextSelectionNavigation

An interface you use to expose methods for obtaining results from actions performed on text selections.

