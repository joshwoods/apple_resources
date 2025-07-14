

- Foundation
-  Morphology 

Structure

# Morphology

A description of the grammatical properties of a string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Morphology
```

## Overview

Use a morphology with an InflectionRule to specify how to interpret a specific word when inflecting an AttributedString. This affects grammatical agreement with traits like number and gender, as well as declaring the word’s part of speech.

The Morphology type’s design is language-independent; the concepts it can specify encompass the spectrum of what languages can do. Even for languages that don’t have one or more of those properties benefit the system as hints to make appropriate choices even when an exact inflection isn’t possible. Examples of properties absent from languages include Spanish’s lack of a grammatical gender of neuter, or the nonexistence of a paucal (plural few) pronoun in English.

## Topics

### Creating a Morphology Instance

init()

Creates an empty morphology instance.

### Accessing the User’s Morphology

static let user: Morphology

The addressing preferences of the current user.

### Accessing Grammatical Properties

var isUnspecified: Bool

A Boolean value that indicates whether this instance specifies no particular grammar.

var grammaticalGender: Morphology.GrammaticalGender?

The grammatical gender used for inflecting strings with this morphology.

enum GrammaticalGender

A representation of grammatical gender, used for inflecting strings.

var number: Morphology.GrammaticalNumber?

The grammatical number used for inflecting strings with this morphology.

enum GrammaticalNumber

A representation of grammatical number, used for inflecting strings.

var partOfSpeech: Morphology.PartOfSpeech?

The grammatical part of speech used for inflecting strings with this morphology.

enum PartOfSpeech

A representation of grammatical parts of speech, used for inflecting strings.

### Accessing Per-Language Features

func setCustomPronoun(Morphology.CustomPronoun?, forLanguage: String) throws

Sets a custom pronoun behavior for this morphology to apply to the given language.

Deprecated

func customPronoun(forLanguage: String) -> Morphology.CustomPronoun?

Returns any custom pronoun behavior this morphology applies to the given language.

Deprecated

struct CustomPronoun

A custom pronoun behavior for use in a specific langauge.

Deprecated

### Structures

struct Pronoun

A custom pronoun for referring to a third person.

### Instance Properties

var definiteness: Morphology.Definiteness?

var determination: Morphology.Determination?

var grammaticalCase: Morphology.GrammaticalCase?

var grammaticalPerson: Morphology.GrammaticalPerson?

var pronounType: Morphology.PronounType?

### Enumerations

enum Definiteness

enum Determination

enum GrammaticalCase

enum GrammaticalPerson

enum PronounType

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

struct TermOfAddress

A term of address that may be used to refer to a third person

enum InflectionConcept

An inflection method to use when localizing text.

struct Pronoun

A custom pronoun for referring to a third person.

