

- Assignables
- AssignableDocumentConfiguration
-  pointsPerBonusScoreMark 

Instance Property

# pointsPerBonusScoreMark

The value of each bonus score mark in the assessment.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var pointsPerBonusScoreMark: Double { get set }
```

**Required**

## See Also

### Configuring a document

var maxScore: Double?

An optional maximum score for this assessment. If `nil`, this value will be synthesized from the question data and associated annotations.

**Required**

var correctScoreMarkType: AssignableDocument.CorrectMarkType

The glyph to use for a correct score mark in the assessment.

**Required**

var pointsPerCorrectScoreMark: Double

The value of each correct score mark in the assessment.

**Required**

var pointsPerIncorrectScoreMark: Double

The value of each incorrect score mark in the assessment.

**Required**

