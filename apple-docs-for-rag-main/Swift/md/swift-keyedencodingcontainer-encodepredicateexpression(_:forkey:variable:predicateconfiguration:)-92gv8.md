

- Swift
- KeyedEncodingContainer
-  encodePredicateExpression(\_:forKey:variable:predicateConfiguration:) 

Instance Method

# encodePredicateExpression(\_:forKey:variable:predicateConfiguration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func encodePredicateExpression(
    _ expression: T,
    forKey key: KeyedEncodingContainer.Key,
    variable: repeat PredicateExpressions.Variable,
    predicateConfiguration: PredicateCodableConfiguration
) throws where T : PredicateExpression, T : Encodable, T.Output == Bool
```

Available when `K` conforms to `CodingKey`.

