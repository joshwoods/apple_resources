

- Foundation
- PredicateExpressions
-  build_contains(\_:\_:) 

Type Method

# build_contains(\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
static func build_contains(
    _ subject: Subject,
    _ regex: Regex
) -> PredicateExpressions.StringContainsRegex where Subject : PredicateExpression, Regex : PredicateExpression, Subject.Output : BidirectionalCollection, Regex.Output : RegexComponent, Subject.Output.SubSequence == Substring
```

