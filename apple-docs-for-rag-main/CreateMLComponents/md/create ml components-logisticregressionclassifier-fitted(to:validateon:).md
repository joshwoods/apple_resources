

- Create ML Components
- LogisticRegressionClassifier
-  fitted(to:validateOn:) 

Instance Method

# fitted(to:validateOn:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation
) async throws -> Self.Transformer where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
```

