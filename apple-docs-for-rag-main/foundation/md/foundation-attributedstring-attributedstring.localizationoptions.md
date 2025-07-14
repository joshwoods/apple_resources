

- Foundation
- AttributedString
-  AttributedString.LocalizationOptions 

Structure

# AttributedString.LocalizationOptions

Configuration options for the localization of text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LocalizationOptions
```

## Topics

### Initializers

init()

### Instance Properties

var applyReplacementIndexAttribute: Bool

var concepts: [InflectionConcept]?

The inflection concepts for achieving automatic grammar agreement during localization.

var inflect: Bool

var replacements: [any CVarArg]?

### Type Methods

static func localizedPhraseConcept(String) -> AttributedString.LocalizationOptions

static func termsOfAddressConcept([TermOfAddress]) -> AttributedString.LocalizationOptions

