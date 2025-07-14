

- Foundation
- PredicateExpressions
-  build_starts(\_:with:) 

Type Method

# build_starts(\_:with:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func build_starts(
    _ base: Base,
    with prefix: Prefix
) -> PredicateExpressions.SequenceStartsWith where Base : PredicateExpression, Prefix : PredicateExpression, Base.Output : Sequence, Prefix.Output : Sequence, Base.Output.Element : Equatable, Base.Output.Element == Prefix.Output.Element
```

