

- Swift
- StringProtocol
-  range(of:options:range:locale:) 

Instance Method

# range(of:options:range:locale:)

Finds and returns the range of the first occurrence of a given string within a given range of the `String`, subject to given options, using the specified locale, if any.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(
    of aString: T,
    options mask: String.CompareOptions = [],
    range searchRange: Range? = nil,
    locale: Locale? = nil
) -> Range? where T : StringProtocol
```

