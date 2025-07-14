

- Create ML Components
- LogisticRegressionClassifier
-  update(\_:with:) 

Instance Method

# update(\_:with:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout Self.Transformer,
    with input: InputSequence
) async throws where InputSequence : Sequence, InputSequence.Element == AnnotatedFeature
```

