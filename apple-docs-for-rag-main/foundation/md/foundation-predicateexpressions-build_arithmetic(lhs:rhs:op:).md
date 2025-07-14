

- Foundation
- PredicateExpressions
-  build_Arithmetic(lhs:rhs:op:) 

Type Method

# build_Arithmetic(lhs:rhs:op:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Arithmetic(
    lhs: LHS,
    rhs: RHS,
    op: PredicateExpressions.ArithmeticOperator
) -> PredicateExpressions.Arithmetic where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Numeric, LHS.Output == RHS.Output
```

