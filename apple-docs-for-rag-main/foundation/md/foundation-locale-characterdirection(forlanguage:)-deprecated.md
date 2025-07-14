

- Foundation
- Locale
-  characterDirection(forLanguage:) Deprecated

Type Method

# characterDirection(forLanguage:)

Returns the character direction for a specified language code.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 8.0–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0+watchOS 2.0–9.0Deprecated

``` source
static func characterDirection(forLanguage isoLangCode: String) -> Locale.LanguageDirection
```

Deprecated

Use \`Locale.Language(identifier:).characterDirection\`

## See Also

### Getting line and character direction for a language

static func lineDirection(forLanguage: String) -> Locale.LanguageDirection

Returns the line direction for a specified language code.

Deprecated

typealias LanguageDirection

An alias for the standard set of language directions.

enum LanguageDirection

The directions that a language may take across a page of text.

