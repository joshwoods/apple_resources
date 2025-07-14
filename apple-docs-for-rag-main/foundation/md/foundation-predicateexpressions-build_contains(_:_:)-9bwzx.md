

- Foundation
- PredicateExpressions
-  build_contains(\_:\_:) 

Type Method

# build_contains(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_contains(
    _ lhs: LHS,
    _ rhs: RHS
) -> PredicateExpressions.SequenceContains where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output : Equatable, RHS.Output == LHS.Output.Element
```

