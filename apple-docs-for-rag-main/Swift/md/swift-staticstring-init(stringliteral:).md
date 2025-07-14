

- Swift
- StaticString
-  init(stringLiteral:) 

Initializer

# init(stringLiteral:)

Creates an instance initialized to the value of a string literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(stringLiteral value: StaticString)
```

## Discussion

Do not call this initializer directly. It may be used by the compiler when you initialize a static string using a string literal.

