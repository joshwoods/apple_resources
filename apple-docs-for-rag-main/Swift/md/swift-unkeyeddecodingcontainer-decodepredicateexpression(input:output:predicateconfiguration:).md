

- Swift
- UnkeyedDecodingContainer
-  decodePredicateExpression(input:output:predicateConfiguration:) 

Instance Method

# decodePredicateExpression(input:output:predicateConfiguration:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func decodePredicateExpression(
    input: repeat (each Input).Type,
    output: Output.Type,
    predicateConfiguration: PredicateCodableConfiguration
) throws -> (expression: any PredicateExpression, variable: (repeat PredicateExpressions.Variable))
```

