

- Foundation
- PredicateExpressions
-  build_Conditional(\_:\_:\_:) 

Type Method

# build_Conditional(\_:\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_Conditional(
    _ test: Test,
    _ trueBranch: If,
    _ falseBranch: Else
) -> PredicateExpressions.Conditional where Test : PredicateExpression, If : PredicateExpression, Else : PredicateExpression, Test.Output == Bool, If.Output == Else.Output
```

