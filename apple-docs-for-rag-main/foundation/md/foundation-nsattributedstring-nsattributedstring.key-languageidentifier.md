

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  languageIdentifier 

Type Property

# languageIdentifier

The language identifier associated with the range of text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let languageIdentifier: NSAttributedString.Key
```

## Discussion

The value of this property is an NSString with the language identifier code in ISO 639 format.

## See Also

### Getting translation-related attribute keys

static let morphology: NSAttributedString.Key

An attribute that contains grammatical properties to apply to the text.

static let inflectionRule: NSAttributedString.Key

An attribute that tells the system how to apply grammar rules and other modifiers to the range of text.

static let inflectionAlternative: NSAttributedString.Key

The alternative translation for a string when no suitable inflection exists.

static let agreeWithArgument: NSAttributedString.Key

static let agreeWithConcept: NSAttributedString.Key

static let referentConcept: NSAttributedString.Key

static let localizedNumberFormat: NSAttributedString.Key

