

- Foundation
- Data
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all elements from the collection.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

## Parameters 

`keepCapacity`  

Pass `true` to request that the collection avoid releasing its storage. Retaining the collection’s storage can be a useful optimization when you’re planning to grow the collection again. The default value is `false`.

## Discussion

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Removing Bytes

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

