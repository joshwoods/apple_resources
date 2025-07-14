

- Foundation
- NSString
-  localizedLowercase 

Instance Property

# localizedLowercase

Returns a version of the string with all letters converted to lowercase, taking into account the current locale.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizedLowercase: String { get }
```

## Discussion

Case transformations aren’t guaranteed to be symmetrical or to produce strings of the same lengths as the originals. See lowercased for an example.

## See Also

### Changing Case

var lowercased: String

A lowercase representation of the string.

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

