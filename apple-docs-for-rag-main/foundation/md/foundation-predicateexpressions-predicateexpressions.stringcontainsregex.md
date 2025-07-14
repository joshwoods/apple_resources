

- Foundation
- PredicateExpressions
-  PredicateExpressions.StringContainsRegex 

Structure

# PredicateExpressions.StringContainsRegex

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
struct StringContainsRegex where Subject : PredicateExpression, Regex : PredicateExpression, Subject.Output : BidirectionalCollection, Regex.Output : RegexComponent, Subject.Output.SubSequence == Substring
```

## Topics

### Initializers

init(subject: Subject, regex: Regex)

### Instance Properties

let regex: Regex

let subject: Subject

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Subject` conforms to `StandardPredicateExpression`, `Regex` conforms to `StandardPredicateExpression`, `Subject.Output` conforms to `BidirectionalCollection`, `Regex.Output` conforms to `RegexComponent`, and `Subject.Output.SubSequence` is `Substring`.

