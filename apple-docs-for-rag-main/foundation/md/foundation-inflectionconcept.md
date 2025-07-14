

- Foundation
-  InflectionConcept 

Enumeration

# InflectionConcept

An inflection method to use when localizing text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum InflectionConcept
```

## Overview

Use `InflectionConcept` when you want to make a localizable string grammatically agree with a phrase or term of address that isn’t part of the text you’re localizing. Set InflectionConcept on the concepts property of AttributedString.LocalizationOptions to specify the inflection concepts to use while inflecting text.

For examples of how to use inflection concepts, see:

- AttributeScopes.FoundationAttributes.ReferentConceptAttribute

- AttributeScopes.FoundationAttributes.AgreementConceptAttribute

## Topics

### Using inflection concepts

case termsOfAddress([TermOfAddress])

Indicates that the system uses the associated terms of address for grammatical agreement when localizing text.

case localizedPhrase(String)

Indicates that the system uses the associated string for grammatical agreement when localizing text.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Automatic grammar agreement

enum InflectionRule

A rule that affects how an attributed string performs automatic grammatical agreement.

struct Morphology

A description of the grammatical properties of a string.

struct TermOfAddress

A term of address that may be used to refer to a third person

struct Pronoun

A custom pronoun for referring to a third person.

