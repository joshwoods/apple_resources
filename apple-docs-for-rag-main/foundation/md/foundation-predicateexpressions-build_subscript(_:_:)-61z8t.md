

- Foundation
- PredicateExpressions
-  build_subscript(\_:\_:) 

Type Method

# build_subscript(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_subscript(
    _ wrapped: Wrapped,
    _ key: Key
) -> PredicateExpressions.DictionaryKeySubscript where Wrapped : PredicateExpression, Key : PredicateExpression, Wrapped.Output == [Key.Output : Value], Key.Output : Hashable
```

