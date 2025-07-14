

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.AgreementArgumentAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.AgreementArgumentAttribute

An attribute that represents grammatical agreement with an argument in a localized string.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum AgreementArgumentAttribute
```

## Overview

Many languages require grammatical agreement in their sentences. In Spanish, for example, the adjectives and verbs need to agree with the gender of the subject they refer to in the sentence. For example, suppose you need to translate the following sentence into Spanish: *Your small salad is ready.* The correct translation is: *Tu ensalada pequeña está lista.*

The challenge is that, most often, the localization file only contains masculine forms of translated words. So, in this sentence, the masculine words for *small* and *ready*, *pequeño* and *listo*, need to inflect and become *pequeña* and *lista* to agree with the feminine subject of the sentence (*ensalada*).

You can make the first part of the sentence grammatically agree by inflecting the words *ensalada* and *pequeño* together using the `inflect` attribute. Because *ensalada* is the feminine subject of the sentence, masculine *pequeño* inflects to feminine *pequeña*.

\_\_The second part of the sentence, however, requires the `agreeWithArgument` attribute. Although *listo* is at the end of the sentence, it needs to inflect on the subject, *ensalada*, which is at the beginning. By wrapping *listo* in an `agreeWithArgument` attribute and pointing it to the feminine word *ensalada*, masculine *listo* inflects to feminine *lista*, making the entire sentence agree.

Using `agreeWithArgument` this way eliminates the need for the localization file to include both the masculine and the feminine forms of each word. By wrapping the words needing inflection, and then pointing them to the words they need to agree with, the system achieves agreement in the localized text for you.

The following steps ensure proper gender agreement in the translation:

1.  Create a type containing all the words you need for translation. For example, create an `Order` structure containing two localizable string properties for `item` and `size`.

2.  Add the necessary translations for the food items and the sizes into the Spanish localization file.

3.  Create a LocalizedStringResource containing the English key phrase from the Spanish localization file to translate, along with placeholder variables representing the words to inflect (*size* and *item*).

4.  In the Spanish localization file, add `%@` placeholders for the words you want to substitute as part of the translation. Make the Spanish words for the size and the item grammatically agree using the `inflect` attribute with a value of true. Then make the masculine Spanish word for *ready* (*listo*) agree with the feminine word for *salad* (*ensalada*) by wrapping *listo* in an `agreeWithArgument` attribute, pointing to the second replacement in the sentence (*ensalada*). Note how the placeholder attributes for *small salad*, `%1@` and `%2@`, reverse order in the code example below when translating from English to Spanish.

5.  Inflect the entire sentence by passing the LocalizedStringResource instance into a new instance of AttributedString.

```
struct Order {
    let item: String
    let size: String
}

let order = Order(item: String(localized: "salad"), size: String(localized: "small"))

// ____________
// In the Spanish localization file:
// "salad" = "ensalada"
// "small" = "pequeño"
// ____________

// Define the resource you want to apply grammatical agreement to.
let resource = LocalizedStringResource("Your \(order.size) \(order.item) is ready.")

// ____________
// In the Spanish localization file:
// "Your %1@ %2@ is ready." = "Tu ^[%2$@ %1$@](inflect: true) está ^[listo](agreeWithArgument: 2)."
// ____________

// Make a new string imposing grammatical agreement on the resource from the localized phrase.
let result = AttributedString(localized: resource)
// result == "Tu ensalada pequeña está lista."

```

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

