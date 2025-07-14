

- Foundation
-  TermOfAddress 

Structure

# TermOfAddress

A term of address that may be used to refer to a third person

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct TermOfAddress
```

## Overview

Not every term of address can be displayed in every language

## Topics

### Instance Properties

var language: Locale.Language?

The specific language associated with a term of address.

var pronouns: [Morphology.Pronoun]

The pronouns associated with a term of address.

### Type Properties

static let currentUser: TermOfAddress

static let feminine: TermOfAddress

The term of address for representing feminine pronouns and grammatical gender.

static let masculine: TermOfAddress

The term of address for representing masculine pronouns and grammatical gender.

static let neutral: TermOfAddress

The term of address for representing gender-neutral pronouns and grammatical gender.

### Type Methods

static func localized(language: Locale.Language, pronouns: [Morphology.Pronoun]) -> TermOfAddress

Returns a term of address restricted to a specific language for a group of pronouns.

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

enum InflectionRule

A rule that affects how an attributed string performs automatic grammatical agreement.

struct Morphology

A description of the grammatical properties of a string.

enum InflectionConcept

An inflection method to use when localizing text.

struct Pronoun

A custom pronoun for referring to a third person.

