

- Swift
- Character
-  Character.UnicodeScalarView 

Type Alias

# Character.UnicodeScalarView

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias UnicodeScalarView = String.UnicodeScalarView
```

## See Also

### Working with a Character’s Unicode Values

init(Unicode.Scalar)

Creates a character containing the given Unicode scalar value.

var unicodeScalars: Character.UnicodeScalarView

var isASCII: Bool

A Boolean value indicating whether this is an ASCII character.

var asciiValue: UInt8?

The ASCII encoding value of this character, if it is an ASCII character.

