

- Swift
- Set
-  remove(at:) 

Instance Method

# remove(at:)

Removes the element at the given index of the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(at position: Set.Index) -> Element
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`position`  

The index of the member to remove. `position` must be a valid index of the set, and must not be equal to the set’s end index.

## Return Value

The element that was removed from the set.

## See Also

### Removing Elements

func filter((Element) throws -> Bool) rethrows -> Set&lt;Element>

Returns a new set containing the elements of the set that satisfy the given predicate.

func remove(Element) -> Element?

Removes the specified element from the set.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func removeFirst() -> Element

Removes the first element of the set.

func removeAll(keepingCapacity: Bool)

Removes all members from the set.

