

- Foundation
- PredicateExpressions
-  build_allSatisfy(\_:\_:) 

Type Method

# build_allSatisfy(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_allSatisfy(
    _ lhs: LHS,
    _ builder: (PredicateExpressions.Variable) -> RHS
) -> PredicateExpressions.SequenceAllSatisfy where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output == Bool
```

