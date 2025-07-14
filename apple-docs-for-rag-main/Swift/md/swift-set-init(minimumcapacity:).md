

- Swift
- Set
-  init(minimumCapacity:) 

Initializer

# init(minimumCapacity:)

Creates an empty set with preallocated space for at least the specified number of elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(minimumCapacity: Int)
```

## Parameters 

`minimumCapacity`  

The minimum number of elements that the newly created set should be able to store without reallocating its storage buffer.

## Discussion

Use this initializer to avoid intermediate reallocations of a set’s storage buffer when you know how many elements you’ll insert into the set after creation.

## See Also

### Creating a Set

init()

Creates an empty set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init&lt;Source>(Source)

Creates a new set from a finite sequence of items.

