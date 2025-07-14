

- Foundation
- Morphology
-  Morphology.GrammaticalGender 

Enumeration

# Morphology.GrammaticalGender

A representation of grammatical gender, used for inflecting strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum GrammaticalGender
```

## Topics

### Determining Grammatical Gender

case feminine

The feminine grammatical gender.

case masculine

The masculine grammatical gender.

case neuter

A value to not specify gender when inflecting a string.

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

var number: Morphology.GrammaticalNumber?

The grammatical number used for inflecting strings with this morphology.

enum GrammaticalNumber

A representation of grammatical number, used for inflecting strings.

var partOfSpeech: Morphology.PartOfSpeech?

The grammatical part of speech used for inflecting strings with this morphology.

enum PartOfSpeech

A representation of grammatical parts of speech, used for inflecting strings.

