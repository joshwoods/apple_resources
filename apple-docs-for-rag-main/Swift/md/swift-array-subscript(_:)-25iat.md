

- Swift
- Array
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(index: Int) -> Element { get set }
```

## Parameters 

`index`  

The position of the element to access. `index` must be greater than or equal to `startIndex` and less than `endIndex`.

## Overview

The following example uses indexed subscripting to update an array’s second element. After assigning the new value (`"Butler"`) at a specific position, that value is immediately available at that same position.

```
var streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
streets[1] = "Butler"
print(streets[1])
// Prints "Butler"
```

Complexity

Reading an element from an array is O(1). Writing is O(1) unless the array’s storage is shared with another array or uses a bridged `NSArray` instance as its storage, in which case writing is O(*n*), where *n* is the length of the array.

## See Also

### Accessing Elements

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

subscript(Range&lt;Int>) -> ArraySlice&lt;Element>

Accesses a contiguous subrange of the array’s elements.

subscript&lt;R>(R) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

