

- Foundation
- Morphology
-  isUnspecified 

Instance Property

# isUnspecified

A Boolean value that indicates whether this instance specifies no particular grammar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var isUnspecified: Bool { get }
```

## Discussion

This value is equivalent to having set none of the properties in this Morphology. This occurs when the user hasn’t specified preferences, or chose not to share them with this app. When the morphology is unspecified, inflecting a string with this morphology does nothing.

## See Also

### Accessing Grammatical Properties

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

