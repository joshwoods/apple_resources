

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute

An attribute that provides an alternative inflection phrase when the system can’t achieve grammatical agreement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum InflectionAlternativeAttribute
```

## Overview

Use the `inflectionAlternativeAttribute` to provide an alternative phrase for cases where the system can’t achieve unambiguous grammatical agreement.

For example, suppose you want to inflect the masculine form for *welcome* in Spanish, *bienvenido*, but the system doesn’t know the person’s preferred terms of address. Add an `inflectionAlternative` to your LocalizedStringResource, setting the alternative word or phrase in single quotation marks. The system uses the alternative when it can’t determine proper grammatical agreement.

```
// Define the resource with an inflection alternative.
let resource = LocalizedStringResource("^[Bienvenido](inflect: true, inflectionAlternative: 'Te damos la bienvenida').")

// Use the inflection alternative when the system can't determine agreement.
let result = AttributedString(localized: resource)
// result == "Te damos la bienvenida."
```

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey

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

enum ReferentConceptAttribute

An attribute that specifies a grammatical agreement concept for substituting pronouns in localized text.

let inflectionAlternative: AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute

A scope for accessing an inflection alternative attribute.

