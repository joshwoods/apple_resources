

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.Notation
-  compactName 

Type Property

# compactName

A locale-appropriate compact name notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var compactName: NumberFormatStyleConfiguration.Notation { get }
```

## Discussion

A compact name notation, when available in the format style’s locale, that uses prefixes or suffixes corresponding to powers of ten. The following example shows a compact name notation in the `fr_FR` locale:

```
let compactNameFormatted = 1234.formatted(.number
    .locale(Locale(identifier: "fr_FR"))
    .notation(.compactName)) // "1,2 k"
```

## See Also

### Notations

static var automatic: NumberFormatStyleConfiguration.Notation

A notation that automatically provides locale-appropriate behavior.

static var scientific: NumberFormatStyleConfiguration.Notation

A notation constant that formats values with scientific notation.

