

- Swift
- Set
-  firstIndex(of:) 

Instance Method

# firstIndex(of:)

Returns the index of the given element in the set, or `nil` if the element is not a member of the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func firstIndex(of member: Element) -> Set.Index?
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`member`  

An element to search for in the set.

## Return Value

The index of `member` if it exists in the set; otherwise, `nil`.

## Discussion

Complexity

O(1)

## See Also

### Finding Elements

subscript(Set&lt;Element>.Index) -> Element

Accesses the member at the given position.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

