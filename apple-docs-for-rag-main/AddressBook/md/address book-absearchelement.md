

- Address Book
-  ABSearchElement 

Class

# ABSearchElement

An object you use to specify a search query for records in the Address Book database.

macOS

``` source
class ABSearchElement
```

## Overview

The `ABSearchElement` class is “toll-free bridged” with its procedural C opaque-type counterpart. This means that the `ABSearchElementRef` type is interchangeable in function or method calls with instances of the `ABSearchElement` class.

## Topics

### Searching

init!(forConjunction: ABSearchConjunction, children: [Any]!)

Returns a compound search element, created by combining the search elements in an array with the given conjunction.

### Matching

func matchesRecord(ABRecord!) -> Bool

Tests whether or not a record matches a search element.

### Constants

typealias ABSearchConjunction

Constants used to create compound search elements.

typealias ABSearchComparison

Constants used to specify the type of comparison beingmade.

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

### Search Elements

class ABSearchElementRef

A reference to an ABSearchElement object.

