

- Foundation
- PredicateExpressions
-  build_flatMap(\_:\_:) 

Type Method

# build_flatMap(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_flatMap(
    _ wrapped: LHS,
    _ builder: (PredicateExpressions.Variable) -> RHS
) -> PredicateExpressions.OptionalFlatMap where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output == Wrapped?, RHS.Output == Result?
```

