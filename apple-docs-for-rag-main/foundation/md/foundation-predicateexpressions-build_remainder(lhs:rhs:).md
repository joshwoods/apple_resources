

- Foundation
- PredicateExpressions
-  build_Remainder(lhs:rhs:) 

Type Method

# build_Remainder(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Remainder(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.IntRemainder where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : BinaryInteger, LHS.Output == RHS.Output
```

