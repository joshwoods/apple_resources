

- Foundation
- PredicateExpressions
-  build_Equal(lhs:rhs:) 

Type Method

# build_Equal(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Equal(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.Equal where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Equatable, LHS.Output == RHS.Output
```

