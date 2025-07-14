

- Foundation
- Morphology
- Morphology.CustomPronoun
-  requiredKeys(forLanguage:) Deprecated

Type Method

# requiredKeys(forLanguage:)

Returns a collection of the custom pronoun keys required by this language.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
static func requiredKeys(forLanguage language: String) -> [PartialKeyPath]
```

Deprecated

Use TermOfAddress instead

## Parameters 

`language`  

The language to create a custom pronoun for.

## Return Value

The keys required for the given language.

## Discussion

If any of the required keys for a given language are unset, calling setCustomPronoun(_:forLanguage:) for that language with an incomplete Morphology.CustomPronoun instance throws an error.

## See Also

### Assessing Custom Pronoun Support

static func isSupported(forLanguage: String) -> Bool

Returns a Boolean value that indicates whether the given language supports setting custom pronouns.

Deprecated

