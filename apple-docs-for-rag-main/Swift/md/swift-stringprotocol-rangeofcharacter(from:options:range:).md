

- Swift
- StringProtocol
-  rangeOfCharacter(from:options:range:) 

Instance Method

# rangeOfCharacter(from:options:range:)

Finds and returns the range in the `String` of the first character from a given character set found in a given range with given options.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfCharacter(
    from aSet: CharacterSet,
    options mask: String.CompareOptions = [],
    range aRange: Range? = nil
) -> Range?
```

