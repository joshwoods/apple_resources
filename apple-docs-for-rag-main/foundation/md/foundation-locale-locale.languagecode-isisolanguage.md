

- Foundation
- Locale
- Locale.LanguageCode
-  isISOLanguage 

Instance Property

# isISOLanguage

A Boolean value that indicates whether this language code is in the list of ISO-defined languages.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isISOLanguage: Bool { get }
```

## Discussion

The following code snippet illustrates use of the isISOLanguage value.

```
let enIsISO = Locale.LanguageCode("en").isISOLanguage // true
let gibberishIsISO = Locale.LanguageCode("gibberish").isISOLanguage // false
```

## See Also

### Examining language code properties

var identifier: String

The identifier used to create the language code.

