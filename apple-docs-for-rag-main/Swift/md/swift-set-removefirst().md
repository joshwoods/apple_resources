

- Swift
- Set
-  removeFirst() 

Instance Method

# removeFirst()

Removes the first element of the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func removeFirst() -> Element
```

Available when `Element` conforms to `Hashable`.

## Return Value

A member of the set.

## Discussion

Because a set is not an ordered collection, the “first” element may not be the first element that was added to the set. The set must not be empty.

Complexity

Amortized O(1) if the set does not wrap a bridged `NSSet`. If the set wraps a bridged `NSSet`, the performance is unspecified.

## See Also

### Removing Elements

func filter((Element) throws -> Bool) rethrows -> Set&lt;Element>

Returns a new set containing the elements of the set that satisfy the given predicate.

func remove(Element) -> Element?

Removes the specified element from the set.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func remove(at: Set&lt;Element>.Index) -> Element

Removes the element at the given index of the set.

func removeAll(keepingCapacity: Bool)

Removes all members from the set.

