

- Swift
- KeyedDecodingContainer
-  decodePredicateExpression(forKey:input:predicateConfiguration:) 

Instance Method

# decodePredicateExpression(forKey:input:predicateConfiguration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func decodePredicateExpression(
    forKey key: KeyedDecodingContainer.Key,
    input: repeat (each Input).Type,
    predicateConfiguration: PredicateCodableConfiguration
) throws -> (expression: any PredicateExpression, variable: (repeat PredicateExpressions.Variable))
```

Available when `K` conforms to `CodingKey`.

