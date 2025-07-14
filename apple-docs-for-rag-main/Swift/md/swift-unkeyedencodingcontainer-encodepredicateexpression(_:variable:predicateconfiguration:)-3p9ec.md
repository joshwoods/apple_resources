

- Swift
- UnkeyedEncodingContainer
-  encodePredicateExpression(\_:variable:predicateConfiguration:) 

Instance Method

# encodePredicateExpression(\_:variable:predicateConfiguration:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func encodePredicateExpression(
    _ expression: T,
    variable: repeat PredicateExpressions.Variable,
    predicateConfiguration: PredicateCodableConfiguration
) throws where T : PredicateExpression, T : Encodable
```

