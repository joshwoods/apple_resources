

- Foundation
- Morphology
-  customPronoun(forLanguage:) Deprecated

Instance Method

# customPronoun(forLanguage:)

Returns any custom pronoun behavior this morphology applies to the given language.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
func customPronoun(forLanguage language: String) -> Morphology.CustomPronoun?
```

Deprecated

Use TermOfAddress instead

## Parameters 

`language`  

The language to query for any custom pronoun behavior.

## Return Value

A Morphology.CustomPronoun behavior this morphology uses for the given language, or `nil` if the morphology doesn’t have a custom pronoun behavior set.

## See Also

### Accessing Per-Language Features

func setCustomPronoun(Morphology.CustomPronoun?, forLanguage: String) throws

Sets a custom pronoun behavior for this morphology to apply to the given language.

Deprecated

struct CustomPronoun

A custom pronoun behavior for use in a specific langauge.

Deprecated

