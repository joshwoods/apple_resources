

- Swift
- Set
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified element from the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(_ member: Element) -> Element?
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`member`  

The element to remove from the set.

## Return Value

The value of the `member` parameter if it was a member of the set; otherwise, `nil`.

## Discussion

This example removes the element `"sugar"` from a set of ingredients.

```
var ingredients: Set = ["cocoa beans", "sugar", "cocoa butter", "salt"]
let toRemove = "sugar"
if let removed = ingredients.remove(toRemove) {
    print("The recipe is now \(removed)-free.")
}
// Prints "The recipe is now sugar-free."
```

## See Also

### Removing Elements

func filter((Element) throws -> Bool) rethrows -> Set&lt;Element>

Returns a new set containing the elements of the set that satisfy the given predicate.

func remove&lt;ConcreteElement>(ConcreteElement) -> ConcreteElement?

func removeFirst() -> Element

Removes the first element of the set.

func remove(at: Set&lt;Element>.Index) -> Element

Removes the element at the given index of the set.

func removeAll(keepingCapacity: Bool)

Removes all members from the set.

