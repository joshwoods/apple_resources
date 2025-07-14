

- Swift
- Slice
-  init(base:bounds:) 

Initializer

# init(base:bounds:)

Creates a view into the given collection that allows access to elements within the specified range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    base: Base,
    bounds: Range
)
```

## Parameters 

`base`  

The collection to create a view into.

`bounds`  

The range of indices to allow access to in the new slice.

## Discussion

It is unusual to need to call this method directly. Instead, create a slice of a collection by using the collection’s range-based subscript or by using methods that return a subsequence.

```
let singleDigits = 0...9
let subSequence = singleDigits.dropFirst(5)
print(Array(subSequence))
// Prints "[5, 6, 7, 8, 9]"
```

In this example, the expression `singleDigits.dropFirst(5))` is equivalent to calling this initializer with `singleDigits` and a range covering the last five items of `singleDigits.indices`.

