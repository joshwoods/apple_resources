

- Swift
- Character
-  init(extendedGraphemeClusterLiteral:) 

Initializer

# init(extendedGraphemeClusterLiteral:)

Creates a character with the specified value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(extendedGraphemeClusterLiteral value: Character)
```

## Discussion

Do not call this initializer directly. It is used by the compiler when you use a string literal to initialize a `Character` instance. For example:

```
let oBreve: Character = "o\u{306}"
print(oBreve)
// Prints "ŏ"
```

The assignment to the `oBreve` constant calls this initializer behind the scenes.

## See Also

### Infrequently Used Functionality

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

