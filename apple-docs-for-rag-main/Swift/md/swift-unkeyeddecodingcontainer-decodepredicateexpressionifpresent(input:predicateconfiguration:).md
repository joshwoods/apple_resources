

- Swift
- UnkeyedDecodingContainer
-  decodePredicateExpressionIfPresent(input:predicateConfiguration:) 

Instance Method

# decodePredicateExpressionIfPresent(input:predicateConfiguration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func decodePredicateExpressionIfPresent(
    input: repeat (each Input).Type,
    predicateConfiguration: PredicateCodableConfiguration
) throws -> (expression: any PredicateExpression, variable: (repeat PredicateExpressions.Variable))?
```

