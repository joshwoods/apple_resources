

- Swift
- Array
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance of a collection containing the elements of a sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ elements: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`elements`  

The sequence of elements for the new collection.

## See Also

### Creating an Array

init()

Creates a new, empty array.

init&lt;S>(S)

Creates an array containing the elements of a sequence.

init(repeating: Element, count: Int)

Creates a new array containing the specified number of a single, repeated value.

init(unsafeUninitializedCapacity: Int, initializingWith: (inout UnsafeMutableBufferPointer&lt;Element>, inout Int) throws -> Void) rethrows

Creates an array with the specified capacity, then calls the given closure with a buffer covering the array’s uninitialized memory.

