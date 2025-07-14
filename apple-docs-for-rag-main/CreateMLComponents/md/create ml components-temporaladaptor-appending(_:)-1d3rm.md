

- Create ML Components
- TemporalAdaptor
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this temporal transformer with a transformer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> ComposedTemporalTransformer> where Other : Transformer, Other : Sendable, Self.Output == Other.Input
```

