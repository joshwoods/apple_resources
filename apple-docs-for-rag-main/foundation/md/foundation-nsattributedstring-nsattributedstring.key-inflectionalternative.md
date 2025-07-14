

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  inflectionAlternative 

Type Property

# inflectionAlternative

The alternative translation for a string when no suitable inflection exists.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let inflectionAlternative: NSAttributedString.Key
```

## Discussion

In languages that change the form of words to match someone’s gender, the system can automatically change (or inflect) the gender to match someone’s personal preferences. If a suitable inflection doesn’t exist, the system uses the value of this attribute instead. Add this attribute to specify a suitable translation that applies to anyone. For example, if a language has only masculine and feminine genders, specify an appropriately neutral translation of the text.

The value of this key is an NSString with the replacement phrase to use.

## See Also

### Getting translation-related attribute keys

static let languageIdentifier: NSAttributedString.Key

The language identifier associated with the range of text.

static let morphology: NSAttributedString.Key

An attribute that contains grammatical properties to apply to the text.

static let inflectionRule: NSAttributedString.Key

An attribute that tells the system how to apply grammar rules and other modifiers to the range of text.

static let agreeWithArgument: NSAttributedString.Key

static let agreeWithConcept: NSAttributedString.Key

static let referentConcept: NSAttributedString.Key

static let localizedNumberFormat: NSAttributedString.Key

