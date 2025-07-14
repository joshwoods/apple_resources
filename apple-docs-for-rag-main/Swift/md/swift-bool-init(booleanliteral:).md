

- Swift
- Bool
-  init(booleanLiteral:) 

Initializer

# init(booleanLiteral:)

Creates an instance initialized to the specified Boolean literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(booleanLiteral value: Bool)
```

## Parameters 

`value`  

The value of the new instance.

## Discussion

Do not call this initializer directly. It is used by the compiler when you use a Boolean literal. Instead, create a new `Bool` instance by using one of the Boolean literals `true` or `false`.

```
var printedMessage = false

if !printedMessage {
    print("You look nice today!")
    printedMessage = true
}
// Prints "You look nice today!"
```

In this example, both assignments to the `printedMessage` variable call this Boolean literal initializer behind the scenes.

## See Also

### Infrequently Used Intializers

init()

Creates an instance initialized to `false`.

