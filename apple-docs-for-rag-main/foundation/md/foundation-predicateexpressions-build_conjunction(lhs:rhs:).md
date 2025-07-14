

- Foundation
- PredicateExpressions
-  build_Conjunction(lhs:rhs:) 

Type Method

# build_Conjunction(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Conjunction(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.Conjunction where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output == Bool, RHS.Output == Bool
```

