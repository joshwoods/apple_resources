

- Swift
- KeyedEncodingContainer
-  encodePredicateExpression(\_:forKey:variable:predicateConfiguration:) 

Instance Method

# encodePredicateExpression(\_:forKey:variable:predicateConfiguration:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func encodePredicateExpression(
    _ expression: T,
    forKey key: KeyedEncodingContainer.Key,
    variable: repeat PredicateExpressions.Variable,
    predicateConfiguration: PredicateCodableConfiguration
) throws where T : PredicateExpression, T : Encodable
```

Available when `K` conforms to `CodingKey`.

