

- Foundation
- Morphology
-  Morphology.PartOfSpeech 

Enumeration

# Morphology.PartOfSpeech

A representation of grammatical parts of speech, used for inflecting strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum PartOfSpeech
```

## Topics

### Determining Part of Speech

case determiner

A determiner, as used as a part of speech.

case pronoun

A pronoun, as used as a part of speech.

case letter

A letter, as used as a part of speech.

case adverb

An adverb, as used as a part of speech.

case particle

A particle, as used as a part of speech.

case adjective

An adjective, as used as a part of speech.

case adposition

An adposition, as used as a part of speech.

case verb

A verb, as used as a part of speech.

case noun

A noun, as used as a part of speech.

case conjunction

A conjunction, as used as a part of speech.

case numeral

A numeral, as used as a part of speech.

case interjection

An interjection, as used as a part of speech.

case preposition

A preposition, as used as a part of speech.

case abbreviation

An abbreviation, as used as a part of speech.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

