

- Swift
- Character
-  init(\_:) 

Initializer

# init(\_:)

Creates a character from a single-character string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ s: String)
```

## Parameters 

`s`  

The single-character string to convert to a `Character` instance. `s` must contain exactly one extended grapheme cluster.

## Discussion

The following example creates a new character from the uppercase version of a string that only holds one character.

```
let a = "a"
let capitalA = Character(a.uppercased())
```

