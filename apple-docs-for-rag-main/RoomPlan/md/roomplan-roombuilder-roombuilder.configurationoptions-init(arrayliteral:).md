

- RoomPlan
- RoomBuilder
- RoomBuilder.ConfigurationOptions
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Creates a set containing the elements of the given array literal.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
init(arrayLiteral: Self.Element...)
```

Available when `ArrayLiteralElement` is `Self.Element`.

## Parameters 

`arrayLiteral`  

A list of elements of the new set.

## Discussion

Do not call this initializer directly. It is used by the compiler when you use an array literal. Instead, create a new set using an array literal as its value by enclosing a comma-separated list of values in square brackets. You can use an array literal anywhere a set is expected by the type context.

Here, a set of strings is created from an array literal holding only strings:

```
let ingredients: Set = ["cocoa beans", "sugar", "cocoa butter", "salt"]
if ingredients.isSuperset(of: ["sugar", "salt"]) {
    print("Whatever it is, it's bound to be delicious!")
}
// Prints "Whatever it is, it's bound to be delicious!"
```

