

- Foundation
-  NSOrthography 

Class

# NSOrthography

A description of the linguistic content of natural language text, typically used for spelling and grammar checking.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSOrthography
```

## Overview

Use NSOrthography objects to describe the linguistic content of a piece of text, including which scripts the text contains, a dominant language (and possibly other languages) for each script, and a dominant script and language for the text as a whole.

Scripts are uniformly described by four-letter ISO 15924 script codes, such as `"Latn"`, `"Grek"`, and `"Cyrl"`. The supertags `"Jpan"` and `"Kore"` are typically used for Japanese and Korean text, and `"Hans"` and `"Hant"` are typically used for Chinese text. The tag `"Zyyy"` is used if a specific script cannot be identified. See Internationalization and Localization Guide for more information.

Languages are uniformly described by BCP-47 tags (preferably in canonical form). The tag `"und"` is used if a specific language cannot be determined.

You typically work with orthography objects returned from methods and properties for classes like NSLinguisticTagger and NSSpellChecker.

### Subclassing Notes

Subclasses must override the dominantScript and languageMap properties. These properties are set using init(dominantScript:languageMap:) or orthographyWithDominantScript:languageMap: in Objective-C.

## Topics

### Creating Orthography Objects

class func defaultOrthography(forLanguage: String) -> Self

Creates and returns an orthography object with the default language map for the specified language.

init(dominantScript: String, languageMap: [String : [String]])

Creates an orthography object with the specified dominant script and language map.

### Determining Correspondences Between Languages and Scripts

var languageMap: [String : [String]]

A dictionary that maps script tags to arrays of language tags.

var dominantLanguage: String

The first language in the list of languages for the dominant script.

var dominantScript: String

The dominant script for the text.

func dominantLanguage(forScript: String) -> String?

Returns the dominant language for the specified script.

func languages(forScript: String) -> [String]?

Returns the list of languages for the specified script.

var allScripts: [String]

The scripts appearing as keys in the language map.

var allLanguages: [String]

The languages appearing in values of the language map.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Localization

struct Locale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

func NSLocalizedString(String, tableName: String?, bundle: Bundle, value: String, comment: String) -> String

Returns a localized string from a table that Xcode generates for you when exporting localizations.

struct LocalizedStringResource

A reference to a localizable string, accessible from another process.

protocol CustomLocalizedStringResourceConvertible

A type that provides an out-of-process localizable description.

struct URLResource

A resource located at a particular file URL within a bundle.

