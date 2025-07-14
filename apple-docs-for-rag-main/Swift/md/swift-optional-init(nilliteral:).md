

- Swift
- Optional
-  init(nilLiteral:) 

Initializer

# init(nilLiteral:)

Creates an instance initialized with `nil`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(nilLiteral: ())
```

## Discussion

Do not call this initializer directly. It is used by the compiler when you initialize an `Optional` instance with a `nil` literal. For example:

```
var i: Index? = nil
```

In this example, the assignment to the `i` variable calls this initializer behind the scenes.

## See Also

### Creating a Nil Value

case none

The absence of a value.

