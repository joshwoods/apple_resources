

- Foundation
-  InflectionRule 

Enumeration

# InflectionRule

A rule that affects how an attributed string performs automatic grammatical agreement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum InflectionRule
```

## Overview

Most apps can rely on loading localized strings to perform automatic grammar agreement. Typically, strings in your app’s strings files use the Markdown extension syntax to indicate portions of the string that may require inflection to agree grammatically. This transformation occurs when you load the attributed string with methods like `init(localized:options:table:bundle:locale:comment:)`.

However, if the system lacks information about the words in the string, you may need to apply an inflection rule programmatically. For example, a social networking app may have gender information about other users that you want to apply at runtime. When performing manual inflection at runtime, you use an inflection rule to indicate to the system what portions of a string should be automatically edited, and what to match. Apply the inflect attribute to set an InflectionRule on an AttributedString, then call inflected() to perform the grammar agreement and produce an edited string.

```
var string = AttributedString(localized: "They liked your post.")
// The user who liked the post uses feminine pronouns.
var morphology = Morphology()
morphology.grammaticalGender = .feminine
string.inflect = InflectionRule(morphology: morphology)
let result = string.inflected()
// result == "She liked your post."
```

## Topics

### Creating an Inflection Rule from a Morphology

init(morphology: Morphology)

Creates an inflection rule with the given morphology.

struct Morphology

A description of the grammatical properties of a string.

### Inflection Rule Behaviors

case automatic

An inflection rule that performs automatic grammar agreement with default transformations.

case explicit(Morphology)

An inflection rule that uses a morphology instance to determine how to inflect attribued strings.

### Determining Availability

static func canInflect(language: String) -> Bool

Returns a Boolean value that indicates whether the rule can inflect a given language.

static var canInflectPreferredLocalization: Bool

A Boolean value that indicates whether the rule can inflect the user’s current preferred localization.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Automatic grammar agreement

struct Morphology

A description of the grammatical properties of a string.

struct TermOfAddress

A term of address that may be used to refer to a third person

enum InflectionConcept

An inflection method to use when localizing text.

struct Pronoun

A custom pronoun for referring to a third person.

