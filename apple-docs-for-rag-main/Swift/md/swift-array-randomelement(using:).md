

- Swift
- Array
-  randomElement(using:) 

Instance Method

# randomElement(using:)

Returns a random element of the collection, using the given generator as a source for randomness.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func randomElement(using generator: inout T) -> Self.Element? where T : RandomNumberGenerator
```

## Parameters 

`generator`  

The random number generator to use when choosing a random element.

## Return Value

A random element from the collection. If the collection is empty, the method returns `nil`.

## Discussion

Call `randomElement(using:)` to select a random element from an array or another collection when you are using a custom random number generator. This example picks a name at random from an array:

```
let names = ["Zoey", "Chloe", "Amani", "Amaia"]
let randomName = names.randomElement(using: &myGenerator)!
// randomName == "Amani"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

Note

The algorithm used to select a random element may change in a future version of Swift. If you’re passing a generator that results in the same sequence of elements each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

## See Also

### Accessing Elements

subscript(Int) -> Element

Accesses the element at the specified position.

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

subscript(Range&lt;Int>) -> ArraySlice&lt;Element>

Accesses a contiguous subrange of the array’s elements.

subscript&lt;R>(R) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

func randomElement() -> Self.Element?

Returns a random element of the collection.

