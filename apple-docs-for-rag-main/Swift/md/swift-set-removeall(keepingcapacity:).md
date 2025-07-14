

- Swift
- Set
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all members from the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

Available when `Element` conforms to `Hashable`.

## See Also

### Removing Elements

func filter((Element) throws -> Bool) rethrows -> Set&lt;Element>

Returns a new set containing the elements of the set that satisfy the given predicate.

func remove(Element) -> Element?

Removes the specified element from the set.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func removeFirst() -> Element

Removes the first element of the set.

func remove(at: Set&lt;Element>.Index) -> Element

Removes the element at the given index of the set.

