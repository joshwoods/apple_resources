

- Swift
- StringProtocol
-  commonPrefix(with:options:) 

Instance Method

# commonPrefix(with:options:)

Returns a string containing characters this string and the given string have in common, starting from the beginning of each up to the first characters that aren’t equivalent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func commonPrefix(
    with aString: T,
    options: String.CompareOptions = []
) -> String where T : StringProtocol
```

