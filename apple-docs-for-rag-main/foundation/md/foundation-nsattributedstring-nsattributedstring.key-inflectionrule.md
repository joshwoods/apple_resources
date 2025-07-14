

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  inflectionRule 

Type Property

# inflectionRule

An attribute that tells the system how to apply grammar rules and other modifiers to the range of text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let inflectionRule: NSAttributedString.Key
```

## Discussion

The value of this key is an NSInflectionRule object.

## See Also

### Getting translation-related attribute keys

static let languageIdentifier: NSAttributedString.Key

The language identifier associated with the range of text.

static let morphology: NSAttributedString.Key

An attribute that contains grammatical properties to apply to the text.

static let inflectionAlternative: NSAttributedString.Key

The alternative translation for a string when no suitable inflection exists.

static let agreeWithArgument: NSAttributedString.Key

static let agreeWithConcept: NSAttributedString.Key

static let referentConcept: NSAttributedString.Key

static let localizedNumberFormat: NSAttributedString.Key

