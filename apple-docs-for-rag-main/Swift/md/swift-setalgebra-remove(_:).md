

- Swift
- SetAlgebra
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the given element and any elements subsumed by the given element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(_ member: Self.Element) -> Self.Element?
```

**Required** Default implementation provided.

## Parameters 

`member`  

The element of the set to remove.

## Return Value

For ordinary sets, an element equal to `member` if `member` is contained in the set; otherwise, `nil`. In some cases, a returned element may be distinguishable from `member` by identity comparison or some other means.

For sets where the set type and element type are the same, like `OptionSet` types, this method returns any intersection between the set and `[member]`, or `nil` if the intersection is empty.

## Default Implementations

### SetAlgebra Implementations

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

## See Also

### Adding and Removing Elements

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Inserts the given element in the set if it is not already present.

**Required** Default implementation provided.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set unconditionally.

**Required** Default implementation provided.

