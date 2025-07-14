

- Swift
- Set
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ sequence: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, like an array or a range:

```
let validIndices = Set(0..

## See Also

### Creating a Set

init()

Creates an empty set.

init(minimumCapacity: Int)

Creates an empty set with preallocated space for at least the specified number of elements.

init&lt;Source>(Source)

Creates a new set from a finite sequence of items.

