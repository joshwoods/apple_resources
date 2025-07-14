

- Foundation
- Morphology
-  Morphology.CustomPronoun Deprecated

Structure

# Morphology.CustomPronoun

A custom pronoun behavior for use in a specific langauge.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
struct CustomPronoun
```

Deprecated

Use TermOfAddress instead

## Overview

Set a Morphology.CustomPronoun instance on a Morphology instance when you want to provide a langauge-specific customization of pronoun use in that language. Different languages have different requirements for the grammatical information needed to apply a custom pronoun, so you set custom pronoun behavior on a per-language basis.

The example below shows how to create English “ze” and “hir” custom pronouns:

```
let ze = Morphology.CustomPronoun()
ze.subjectForm = "ze"
ze.objectForm = "hir"
ze.possessiveForm = "hir"
ze.possessiveAdjectiveForm = "hir"
ze.reflexiveForm = "hirself"
```

Morphology.CustomPronoun only supports third-person pronouns. Use this feature when your app needs to refer to third parties with a specific pronoun.

## Topics

### Creating a Custom Pronoun

init()

Creates an empty custom pronoun.

### Assessing Custom Pronoun Support

static func isSupported(forLanguage: String) -> Bool

Returns a Boolean value that indicates whether the given language supports setting custom pronouns.

static func requiredKeys(forLanguage: String) -> [PartialKeyPath&lt;Morphology.CustomPronoun>]

Returns a collection of the custom pronoun keys required by this language.

### Determining Pronoun Forms

var subjectForm: String?

The subject pronoun form to apply when using this custom pronoun behavior.

var objectForm: String?

The object pronoun form to apply when using this custom pronoun behavior.

var possessiveForm: String?

The posessive pronoun form to apply when using this custom pronoun behavior.

var possessiveAdjectiveForm: String?

The posessive adjective pronoun form to apply when using this custom pronoun behavior.

var reflexiveForm: String?

The reflexive pronoun form to apply when using this custom pronoun behavior.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing Per-Language Features

func setCustomPronoun(Morphology.CustomPronoun?, forLanguage: String) throws

Sets a custom pronoun behavior for this morphology to apply to the given language.

Deprecated

func customPronoun(forLanguage: String) -> Morphology.CustomPronoun?

Returns any custom pronoun behavior this morphology applies to the given language.

Deprecated

