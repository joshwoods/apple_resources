

- Foundation
- Data
-  remove(at:) 

Instance Method

# remove(at:)

Removes and returns the element at the specified position.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(at position: Self.Index) -> Self.Element
```

## Parameters 

`position`  

The position of the element to remove. `position` must be a valid index of the collection that is not equal to the collection’s end index.

## Return Value

The removed element.

## Discussion

All the elements following the specified position are moved to close the gap. This example removes the middle element from an array of measurements.

```
var measurements = [1.2, 1.5, 2.9, 1.2, 1.6]
let removed = measurements.remove(at: 2)
print(measurements)
// Prints "[1.2, 1.5, 1.2, 1.6]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Removing Bytes

func removeAll(keepingCapacity: Bool)

Removes all elements from the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

