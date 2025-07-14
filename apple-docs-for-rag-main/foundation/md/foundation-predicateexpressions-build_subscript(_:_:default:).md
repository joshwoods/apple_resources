

- Foundation
- PredicateExpressions
-  build_subscript(\_:\_:default:) 

Type Method

# build_subscript(\_:\_:default:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_subscript(
    _ wrapped: Wrapped,
    _ key: Key,
    default: Default
) -> PredicateExpressions.DictionaryKeyDefaultValueSubscript where Wrapped : PredicateExpression, Key : PredicateExpression, Default : PredicateExpression, Wrapped.Output == [Key.Output : Default.Output], Key.Output : Hashable
```

