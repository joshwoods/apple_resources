

- Swift
- ArraySlice
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Creates an array from the given array literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(arrayLiteral elements: Element...)
```

## Parameters 

`elements`  

A variadic list of elements of the new array.

## Discussion

Do not call this initializer directly. It is used by the compiler when you use an array literal. Instead, create a new array by using an array literal as its value. To do this, enclose a comma-separated list of values in square brackets.

Here, an array of strings is created from an array literal holding only strings:

```
let ingredients: ArraySlice =
      ["cocoa beans", "sugar", "cocoa butter", "salt"]
```

