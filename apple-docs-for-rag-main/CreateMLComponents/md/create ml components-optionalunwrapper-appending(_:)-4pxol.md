

- Create ML Components
- OptionalUnwrapper
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with a temporal transformer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> ComposedTemporalTransformer, Other> where Self : Sendable, Other : TemporalTransformer, Self.Output == Other.Input
```

