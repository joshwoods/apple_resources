

- Foundation
- NSString
-  capitalized 

Instance Property

# capitalized

A capitalized representation of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var capitalized: String { get }
```

## Discussion

A capitalized string is a string with the first character in each word changed to its corresponding uppercase value, and all remaining characters set to their corresponding lowercase values. A word is any sequence of characters delimited by spaces, tabs, or line terminators (listed under getLineStart(_:end:contentsEnd:for:)). Some common word delimiting punctuation isn’t considered, so this property may not generally produce the desired results for multiword strings.

Case transformations aren’t guaranteed to be symmetrical or to produce strings of the same lengths as the originals. See lowercased for an example.

This property performs the canonical (non-localized) mapping. It is suitable for programming operations that require stable results not depending on the current locale.

Important

When working with text that’s presented to the user, use localizedCapitalized or capitalized(with:) instead.

## See Also

### Changing Case

var lowercased: String

A lowercase representation of the string.

var localizedLowercase: String

Returns a version of the string with all letters converted to lowercase, taking into account the current locale.

func lowercased(with: Locale?) -> String

Returns a version of the string with all letters converted to lowercase, taking into account the specified locale.

var uppercased: String

An uppercase representation of the string.

var localizedUppercase: String

Returns a version of the string with all letters converted to uppercase, taking into account the current locale.

func uppercased(with: Locale?) -> String

Returns a version of the string with all letters converted to uppercase, taking into account the specified locale.

var localizedCapitalized: String

Returns a capitalized representation of the receiver using the current locale.

func capitalized(with: Locale?) -> String

Returns a capitalized representation of the receiver using the specified locale.

