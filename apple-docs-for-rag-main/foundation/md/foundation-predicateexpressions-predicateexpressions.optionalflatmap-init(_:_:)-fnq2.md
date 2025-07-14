

- Foundation
- PredicateExpressions
- PredicateExpressions.OptionalFlatMap
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ wrapped: LHS,
    _ builder: (PredicateExpressions.Variable) -> RHS
) where Result == RHS.Output
```

