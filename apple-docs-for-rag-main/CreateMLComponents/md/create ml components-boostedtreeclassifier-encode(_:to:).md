

- Create ML Components
- BoostedTreeClassifier
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: TreeClassifierModel,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding the classifier

func encodeLabels(some Collection&lt;Optional&lt;Label>>) throws -> (labels: [String?], encoded: [Int])

func decode(from: inout any EstimatorDecoder) throws -> TreeClassifierModel&lt;Label>

Decodes a previously fitted transformer.

