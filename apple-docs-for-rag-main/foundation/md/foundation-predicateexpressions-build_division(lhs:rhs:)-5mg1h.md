

- Foundation
- PredicateExpressions
-  build_Division(lhs:rhs:) 

Type Method

# build_Division(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Division(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.FloatDivision where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : FloatingPoint, LHS.Output == RHS.Output
```

