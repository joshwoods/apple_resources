

- Create ML Components
- ImageFeaturePrint
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with an annotated-feature transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some Transformer, Other.Output> where Other : Transformer, Other.Input == AnnotatedFeature
```

