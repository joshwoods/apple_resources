

- AppKit
-  NSTextRange 

Class

# NSTextRange

A class that represents a contiguous range between two locations inside document contents.

macOS 12.0+

``` source
class NSTextRange
```

## Overview

An `NSTextRange` consists of the starting and terminating locations. There the two basic properties: `location` and `endLocation`, respectively. The terminating `location`, `endLocation`, is directly following the last location in the range. For example, a location contains a range if `(range.location 

## Topics

### Creating a text range

convenience init(location: any NSTextLocation)

Creates a new text range at the location you specify.

init?(location: any NSTextLocation, end: (any NSTextLocation)?)

Creates a new text range with the starting and ending locations you specify.

### Characteristics of the text range

var location: any NSTextLocation

Returns the starting location of the text range.

var endLocation: any NSTextLocation

Returns the ending location of the text range.

var isEmpty: Bool

Returns whether the text range is empty.

### Comparing text ranges

func intersection(NSTextRange) -> Self?

Returns the range, if any, where two text ranges intersect.

func intersects(NSTextRange) -> Bool

Determines if two ranges intersect.

func isEqual(to: NSTextRange) -> Bool

Compares two text ranges.

func union(NSTextRange) -> Self

Returns a new text range by forming the union with the text range you provide.

### Finding text within the text range

func contains(any NSTextLocation) -> Bool

Determines if the text location you specify is in the current text range.

func contains(NSTextRange) -> Bool

Determines if the text range you specify is in the current text range.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Location and selection

class NSTextSelection

A class that represents a single logical selection context that corresponds to an insertion point.

class NSTextSelectionNavigation

An interface you use to expose methods for obtaining results from actions performed on text selections.

protocol NSTextLocation

An interface you implement that represents an abstract location inside your document’s content.

