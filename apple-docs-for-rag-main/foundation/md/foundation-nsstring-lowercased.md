

- Foundation
- NSString
-  lowercased 

Instance Property

# lowercased

A lowercase representation of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lowercased: String { get }
```

## Discussion

This property performs the canonical (non-localized) mapping. It is suitable for programming operations that require stable results not depending on the current locale.

Case transformations aren’t guaranteed to be symmetrical or to produce strings of the same lengths as the originals. That is, the result of this statement:

```
lcString = [myString lowercaseString];
```

…might not be equal to this statement:

```
lcString = [[myString uppercaseString] lowercaseString];
```

For example, the uppercase form of “ß” in German is “SS”, so converting “Straße” to uppercase, then lowercase, produces this sequence of strings:

- “Straße”

- “STRASSE”

- “strasse”

Important

When working with text that’s presented to the user, use localizedLowercase or lowercased(with:) instead.

## See Also

### Changing Case

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

var capitalized: String

A capitalized representation of the string.

var localizedCapitalized: String

Returns a capitalized representation of the receiver using the current locale.

func capitalized(with: Locale?) -> String

Returns a capitalized representation of the receiver using the specified locale.

