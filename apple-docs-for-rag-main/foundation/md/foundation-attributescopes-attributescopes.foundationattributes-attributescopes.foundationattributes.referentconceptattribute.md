

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.ReferentConceptAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.ReferentConceptAttribute

An attribute that specifies a grammatical agreement concept for substituting pronouns in localized text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum ReferentConceptAttribute
```

## Overview

Use the referentConcept formatting attribute for cases where you need to refer to a person using their preferred pronoun in a string.

For an example of how to use a `referentConcept`, see TermOfAddress.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey

## See Also

### Using automatic grammar agreement attributes

let inflect: AttributeScopes.FoundationAttributes.InflectionRuleAttribute

A scope for accessing an inflection rule attribute.

enum InflectionRuleAttribute

A type for using an inflection rule as an attribute.

let agreementArgument: AttributeScopes.FoundationAttributes.AgreementArgumentAttribute

A scope for accessing an agreement argument attribute.

enum AgreementArgumentAttribute

An attribute that represents grammatical agreement with an argument in a localized string.

let agreementConcept: AttributeScopes.FoundationAttributes.AgreementConceptAttribute

A scope for accessing an agreement concept attribute.

enum AgreementConceptAttribute

An attribute that represents grammatical agreement for objects that aren’t part of the inflected text.

let morphology: AttributeScopes.FoundationAttributes.MorphologyAttribute

A scope for accessing a morphology attribute.

enum MorphologyAttribute

A type for using a morphology as an attribute.

let referentConcept: AttributeScopes.FoundationAttributes.ReferentConceptAttribute

A scope for accessing a referent concept attribute.

let inflectionAlternative: AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute

A scope for accessing an inflection alternative attribute.

enum InflectionAlternativeAttribute

An attribute that provides an alternative inflection phrase when the system can’t achieve grammatical agreement.

