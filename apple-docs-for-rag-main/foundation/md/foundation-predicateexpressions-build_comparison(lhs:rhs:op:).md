

- Foundation
- PredicateExpressions
-  build_Comparison(lhs:rhs:op:) 

Type Method

# build_Comparison(lhs:rhs:op:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Comparison(
    lhs: LHS,
    rhs: RHS,
    op: PredicateExpressions.ComparisonOperator
) -> PredicateExpressions.Comparison where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Comparable, LHS.Output == RHS.Output
```

