

- Foundation
- Morphology
- Morphology.CustomPronoun
-  isSupported(forLanguage:) Deprecated

Type Method

# isSupported(forLanguage:)

Returns a Boolean value that indicates whether the given language supports setting custom pronouns.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
static func isSupported(forLanguage language: String) -> Bool
```

Deprecated

Use TermOfAddress instead

## Parameters 

`language`  

The language to query.

## Return Value

`true` if the language supports custom pronouns; otherwise, `false`.

## Discussion

If this value is `false` for a given language, calling setCustomPronoun(_:forLanguage:) for that language throws an error.

## See Also

### Assessing Custom Pronoun Support

static func requiredKeys(forLanguage: String) -> [PartialKeyPath&lt;Morphology.CustomPronoun>]

Returns a collection of the custom pronoun keys required by this language.

Deprecated

