

- Swift
- Character
-  asciiValue 

Instance Property

# asciiValue

The ASCII encoding value of this character, if it is an ASCII character.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var asciiValue: UInt8? { get }
```

## Discussion

```
let chars: [Character] = ["a", " ", "™"]
for ch in chars {
    print(ch, "-->", ch.asciiValue)
}
// Prints:
// a --> Optional(97)
//   --> Optional(32)
// ™ --> nil
```

A character with the value “\r\n” (CR-LF) is normalized to “\n” (LF) and has an `asciiValue` property equal to 10.

```
let cr = "\r" as Character
// cr.asciiValue == 13
let lf = "\n" as Character
// lf.asciiValue == 10
let crlf = "\r\n" as Character
// crlf.asciiValue == 10
```

## See Also

### Working with a Character’s Unicode Values

init(Unicode.Scalar)

Creates a character containing the given Unicode scalar value.

var unicodeScalars: Character.UnicodeScalarView

typealias UnicodeScalarView

var isASCII: Bool

A Boolean value indicating whether this is an ASCII character.

