

- Foundation
- AttributeScopes
-  AttributeScopes.FoundationAttributes 

Structure

# AttributeScopes.FoundationAttributes

Attribute scopes that Foundation defines.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FoundationAttributes
```

## Topics

### Using date attributes

let dateField: AttributeScopes.FoundationAttributes.DateFieldAttribute

A property for accessing a date field attribute.

enum DateFieldAttribute

A type for using a date field as an attribute.

### Using language attributes

let languageIdentifier: AttributeScopes.FoundationAttributes.LanguageIdentifierAttribute

A property for accessing a language identifier attribute.

enum LanguageIdentifierAttribute

A type for using a language identifier as an attribute.

### Using URL attributes

let imageURL: AttributeScopes.FoundationAttributes.ImageURLAttribute

A property for accessing an image URL attribute.

enum ImageURLAttribute

A type for using an image URL as an attribute.

let link: AttributeScopes.FoundationAttributes.LinkAttribute

A property for accessing the link attribute.

enum LinkAttribute

A type for using a link as an attribute.

### Using presentation intent attributes

let inlinePresentationIntent: AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute

A property for accessing an inline presentation intent attribute.

enum InlinePresentationIntentAttribute

A type for using an inline presentation intent as an attribute.

struct InlinePresentationIntent

A type that defines presentation intent for runs of characters for traits like emphasis, strikethrough, and code voice.

let presentationIntent: AttributeScopes.FoundationAttributes.PresentationIntentAttribute

A property for accessing a presentation intent attribute.

enum PresentationIntentAttribute

A type for using a presentation intent as an attribute.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

### Using alternative description attributes

let alternateDescription: AttributeScopes.FoundationAttributes.AlternateDescriptionAttribute

A property for accessing an alternative presentation attribute.

enum AlternateDescriptionAttribute

A type for using an alternative description as an attribute.

### Using string formatting attributes

let replacementIndex: AttributeScopes.FoundationAttributes.ReplacementIndexAttribute

A property for accessing a replacement index attribute.

enum ReplacementIndexAttribute

A type for using a replacement index as an attribute.

### Using string localization attributes

let localizedStringArgumentAttributes: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes

A property for accessing a localized string argument attribute.

struct LocalizedStringArgumentAttributes

A type for using a localized string argument as an attribute.

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

enum InflectionAlternativeAttribute

An attribute that provides an alternative inflection phrase when the system can’t achieve grammatical agreement.

### Using number formatting attributes

let numberFormat: AttributeScopes.FoundationAttributes.NumberFormatAttributes

A property for accessing a number format attribute.

struct NumberFormatAttributes

A type for using a number format as an attribute.

### Using person name component attributes

let personNameComponent: AttributeScopes.FoundationAttributes.PersonNameComponentAttribute

A property for accessing a person name component attribute.

enum PersonNameComponentAttribute

A type for using a person name component as an attribute.

### Using Markdown source position attributes

let markdownSourcePosition: AttributeScopes.FoundationAttributes.MarkdownSourcePositionAttribute

A property for accessing a Markdown source position attribute.

enum MarkdownSourcePositionAttribute

A type for using a markdown source position as an attribute.

### Structures

struct MeasurementAttribute

### Instance Properties

let byteCount: AttributeScopes.FoundationAttributes.ByteCountAttribute

let durationField: AttributeScopes.FoundationAttributes.DurationFieldAttribute

let localizedNumberFormat: AttributeScopes.FoundationAttributes.LocalizedNumberFormatAttribute

let measurement: AttributeScopes.FoundationAttributes.MeasurementAttribute

### Enumerations

enum ByteCountAttribute

enum DurationFieldAttribute

enum LocalizedNumberFormatAttribute

## Relationships

### Conforms To

- AttributeScope
- DecodingConfigurationProviding
- EncodingConfigurationProviding

## See Also

### Foundation-Defined Attributes

var foundation: AttributeScopes.FoundationAttributes.Type

A property for accessing the attribute scopes that Foundation defines.

