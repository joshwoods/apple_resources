

- Assignables
-  AssignableDocumentConfiguration 

Protocol

# AssignableDocumentConfiguration

A type that specifies the options for an assignable document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol AssignableDocumentConfiguration : Hashable
```

## Topics

### Configuring a document

var maxScore: Double?

An optional maximum score for this assessment. If `nil`, this value will be synthesized from the question data and associated annotations.

**Required**

var correctScoreMarkType: AssignableDocument.CorrectMarkType

The glyph to use for a correct score mark in the assessment.

**Required**

var pointsPerBonusScoreMark: Double

The value of each bonus score mark in the assessment.

**Required**

var pointsPerCorrectScoreMark: Double

The value of each correct score mark in the assessment.

**Required**

var pointsPerIncorrectScoreMark: Double

The value of each incorrect score mark in the assessment.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable

## See Also

### Configuration

protocol AssignedWorkDocumentConfiguration

A type that specifies the score of a document.

