

- Foundation
- PredicateExpressions
-  build_Disjunction(lhs:rhs:) 

Type Method

# build_Disjunction(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Disjunction(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.Disjunction where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output == Bool, RHS.Output == Bool
```

