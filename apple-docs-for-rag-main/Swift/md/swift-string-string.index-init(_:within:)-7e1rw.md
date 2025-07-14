

- Swift
- String
- String.Index
-  init(\_:within:) 

Initializer

# init(\_:within:)

Creates an index in the given Unicode scalars view that corresponds exactly to the specified `UTF16View` position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    _ sourcePosition: String.Index,
    within unicodeScalars: String.UnicodeScalarView
)
```

## Parameters 

`sourcePosition`  

A position in the `utf16` view of a string. `utf16Index` must be an element of `String(unicodeScalars).utf16.indices`.

`unicodeScalars`  

The `UnicodeScalarView` in which to find the new position.

## Discussion

The following example finds the position of a space in a string’s `utf16` view and then converts that position to an index in the string’s `unicodeScalars` view:

```
let cafe = "Café 🍵"

let utf16Index = cafe.utf16.firstIndex(of: 32)!
let scalarIndex = String.Index(utf16Index, within: cafe.unicodeScalars)!

print(String(cafe.unicodeScalars[..

If the index passed as `sourcePosition` doesn’t have an exact corresponding position in `unicodeScalars`, the result of the initializer is `nil`. For example, an attempt to convert the position of the trailing surrogate of a UTF-16 surrogate pair results in `nil`.

