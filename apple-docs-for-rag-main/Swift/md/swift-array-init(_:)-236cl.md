

- Swift
- Array
-  init(\_:) 

Initializer

# init(\_:)

Creates an array containing the elements of a sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ s: S) where Element == S.Element, S : Sequence
```

## Parameters 

`s`  

The sequence of elements to turn into an array.

## Discussion

You can use this initializer to create an array from any other type that conforms to the `Sequence` protocol. For example, you might want to create an array with the integers from 1 through 7. Use this initializer around a range instead of typing all those numbers in an array literal.

```
let numbers = Array(1...7)
print(numbers)
// Prints "[1, 2, 3, 4, 5, 6, 7]"
```

You can also use this initializer to convert a complex sequence or collection type back to an array. For example, the `keys` property of a dictionary isn’t an array with its own storage, it’s a collection that maps its elements from the dictionary only when they’re accessed, saving the time and space needed to allocate an array. If you need to pass those keys to a method that takes an array, however, use this initializer to convert that list from its type of `LazyMapCollection, Int>` to a simple `[String]`.

```
func cacheImages(withNames names: [String]) {
    // custom image loading and caching
 }

let namedHues: [String: Int] = ["Vermillion": 18, "Magenta": 302,
        "Gold": 50, "Cerise": 320]
let colorNames = Array(namedHues.keys)
cacheImages(withNames: colorNames)

print(colorNames)
// Prints "["Gold", "Cerise", "Magenta", "Vermillion"]"
```

## See Also

### Creating an Array

init()

Creates a new, empty array.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init(repeating: Element, count: Int)

Creates a new array containing the specified number of a single, repeated value.

init(unsafeUninitializedCapacity: Int, initializingWith: (inout UnsafeMutableBufferPointer&lt;Element>, inout Int) throws -> Void) rethrows

Creates an array with the specified capacity, then calls the given closure with a buffer covering the array’s uninitialized memory.

