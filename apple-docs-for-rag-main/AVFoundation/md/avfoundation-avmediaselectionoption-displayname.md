

- AVFoundation
- AVMediaSelectionOption
-  displayName 

Instance Property

# displayName

A string suitable for display using the current system locale.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var displayName: String { get }
```

## Discussion

The string takes into account this option’s common metadata, media characteristics, and locale properties in addition to the provided locale to formulate a string intended for display

## See Also

### Getting the Language and Locale Settings

func displayName(with: Locale) -> String

Returns a string suitable for display using the specified locale.

var locale: Locale?

The locale for which the media option was authored.

var extendedLanguageTag: String?

The IETF BCP 47 language tag associated with the option

