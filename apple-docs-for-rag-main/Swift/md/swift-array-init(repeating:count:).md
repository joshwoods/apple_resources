

- Swift
- Array
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Creates a new array containing the specified number of a single, repeated value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    repeating repeatedValue: Element,
    count: Int
)
```

## Parameters 

`repeatedValue`  

The element to repeat.

`count`  

The number of times to repeat the value passed in the `repeating` parameter. `count` must be zero or greater.

## Discussion

Here’s an example of creating an array initialized with five strings containing the letter *Z*.

```
let fiveZs = Array(repeating: "Z", count: 5)
print(fiveZs)
// Prints "["Z", "Z", "Z", "Z", "Z"]"
```

## See Also

### Creating an Array

init()

Creates a new, empty array.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init&lt;S>(S)

Creates an array containing the elements of a sequence.

init(unsafeUninitializedCapacity: Int, initializingWith: (inout UnsafeMutableBufferPointer&lt;Element>, inout Int) throws -> Void) rethrows

Creates an array with the specified capacity, then calls the given closure with a buffer covering the array’s uninitialized memory.

