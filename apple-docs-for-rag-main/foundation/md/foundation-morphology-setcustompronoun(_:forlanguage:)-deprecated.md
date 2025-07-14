

- Foundation
- Morphology
-  setCustomPronoun(\_:forLanguage:) Deprecated

Instance Method

# setCustomPronoun(\_:forLanguage:)

Sets a custom pronoun behavior for this morphology to apply to the given language.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
mutating func setCustomPronoun(
    _ pronoun: Morphology.CustomPronoun?,
    forLanguage language: String
) throws
```

Deprecated

Use TermOfAddress instead

## Parameters 

`pronoun`  

A Morphology.CustomPronoun instance for the morphology to use.

`language`  

The language the morphology should apply the custom pronoun to.

## Discussion

This method throws if the system doesn’t support custom pronouns for the given language, or if any of the required pronoun keys aren’t set.

## See Also

### Related Documentation

static func isSupported(forLanguage: String) -> Bool

Returns a Boolean value that indicates whether the given language supports setting custom pronouns.

Deprecated

static func requiredKeys(forLanguage: String) -> [PartialKeyPath&lt;Morphology.CustomPronoun>]

Returns a collection of the custom pronoun keys required by this language.

Deprecated

### Accessing Per-Language Features

func customPronoun(forLanguage: String) -> Morphology.CustomPronoun?

Returns any custom pronoun behavior this morphology applies to the given language.

Deprecated

struct CustomPronoun

A custom pronoun behavior for use in a specific langauge.

Deprecated

