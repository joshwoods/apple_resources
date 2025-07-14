

- Swift
- Set
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns a new set containing the elements of the set that satisfy the given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+Swift 4.0+

``` source
func filter(_ isIncluded: (Element) throws -> Bool) rethrows -> Set
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`isIncluded`  

A closure that takes an element as its argument and returns a Boolean value indicating whether the element should be included in the returned set.

## Return Value

A set of the elements that `isIncluded` allows.

## Discussion

In this example, `filter(_:)` is used to include only names shorter than five characters.

```
let cast: Set = ["Vivien", "Marlon", "Kim", "Karl"]
let shortNames = cast.filter { $0.count 

## See Also

### Removing Elements

func remove(Element) -> Element?

Removes the specified element from the set.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func removeFirst() -> Element

Removes the first element of the set.

func remove(at: Set&lt;Element>.Index) -> Element

Removes the element at the given index of the set.

func removeAll(keepingCapacity: Bool)

Removes all members from the set.

