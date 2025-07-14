

- Swift
- StringProtocol
-  compare(\_:options:range:locale:) 

Instance Method

# compare(\_:options:range:locale:)

Compares the string using the specified options and returns the lexical ordering for the range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(
    _ aString: T,
    options mask: String.CompareOptions = [],
    range: Range? = nil,
    locale: Locale? = nil
) -> ComparisonResult where T : StringProtocol
```

