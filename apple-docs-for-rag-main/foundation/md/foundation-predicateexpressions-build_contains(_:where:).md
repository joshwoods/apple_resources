

- Foundation
- PredicateExpressions
-  build_contains(\_:where:) 

Type Method

# build_contains(\_:where:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_contains(
    _ lhs: LHS,
    where builder: (PredicateExpressions.Variable) -> RHS
) -> PredicateExpressions.SequenceContainsWhere where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output == Bool
```

