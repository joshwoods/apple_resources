

- Swift
- Set
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Creates a set containing the elements of the given array literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(arrayLiteral elements: Element...)
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`elements`  

A variadic list of elements of the new set.

## Discussion

Do not call this initializer directly. It is used by the compiler when you use an array literal. Instead, create a new set using an array literal as its value by enclosing a comma-separated list of values in square brackets. You can use an array literal anywhere a set is expected by the type context.

Here, a set of strings is created from an array literal holding only strings.

```
let ingredients: Set = ["cocoa beans", "sugar", "cocoa butter", "salt"]
if ingredients.isSuperset(of: ["sugar", "salt"]) {
    print("Whatever it is, it's bound to be delicious!")
}
// Prints "Whatever it is, it's bound to be delicious!"
```

## See Also

### Infrequently Used Functionality

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

