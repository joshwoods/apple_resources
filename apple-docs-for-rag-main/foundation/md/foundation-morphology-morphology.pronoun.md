

- Foundation
- Morphology
-  Morphology.Pronoun 

Structure

# Morphology.Pronoun

A custom pronoun for referring to a third person.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Pronoun
```

## Overview

Create instances of Morphology.Pronoun when you need to define custom pronouns for a localized term of address.

For examples of how to create custom pronouns, see TermOfAddress.

## Topics

### Creating pronouns

init(pronoun: String, morphology: Morphology, dependentMorphology: Morphology?)

Creates a pronoun with the specified name, morphology, and dependent morphology.

### Using pronouns

var pronoun: String

The string representation of the pronoun.

var morphology: Morphology

The morphology of the pronoun form.

var dependentMorphology: Morphology?

The dependent morphology of the pronoun form.

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

struct TermOfAddress

A term of address that may be used to refer to a third person

enum InflectionConcept

An inflection method to use when localizing text.

