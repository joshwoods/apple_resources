

- Foundation
- PredicateExpressions
-  build_filter(\_:\_:) 

Type Method

# build_filter(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_filter(
    _ lhs: LHS,
    _ builder: (PredicateExpressions.Variable) -> RHS
) -> PredicateExpressions.Filter where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output == Bool
```

