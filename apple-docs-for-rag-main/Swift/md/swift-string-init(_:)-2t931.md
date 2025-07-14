

- Swift
- String
-  init(\_:) 

Initializer

# init(\_:)

Creates a string corresponding to the given collection of Unicode scalars.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ unicodeScalars: String.UnicodeScalarView)
```

## Parameters 

`unicodeScalars`  

A collection of Unicode scalar values.

## Discussion

You can use this initializer to create a new string from a slice of another string’s `unicodeScalars` view.

```
let picnicGuest = "Deserving porcupine"
if let i = picnicGuest.unicodeScalars.firstIndex(of: " ") {
    let adjective = String(picnicGuest.unicodeScalars[..

The `adjective` constant is created by calling this initializer with a slice of the `picnicGuest.unicodeScalars` view.

## See Also

### Working with String Views

var unicodeScalars: String.UnicodeScalarView

The string’s value represented as a collection of Unicode scalar values.

init(Substring.UnicodeScalarView)

Creates a String having the given content.

var utf16: String.UTF16View

A UTF-16 encoding of `self`.

init(String.UTF16View)

Creates a string corresponding to the given sequence of UTF-16 code units.

init?(Substring.UTF16View)

Creates a String having the given content.

var utf8: String.UTF8View

A UTF-8 encoding of `self`.

init(String.UTF8View)

Creates a string corresponding to the given sequence of UTF-8 code units.

init?(Substring.UTF8View)

Creates a String having the given content.

