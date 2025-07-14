

- Foundation
- PredicateExpressions
-  build_NotEqual(lhs:rhs:) 

Type Method

# build_NotEqual(lhs:rhs:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_NotEqual(
    lhs: LHS,
    rhs: RHS
) -> PredicateExpressions.NotEqual where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Equatable, LHS.Output == RHS.Output
```

