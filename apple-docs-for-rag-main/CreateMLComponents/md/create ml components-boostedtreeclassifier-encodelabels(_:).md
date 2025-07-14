

- Create ML Components
- BoostedTreeClassifier
-  encodeLabels(\_:) 

Instance Method

# encodeLabels(\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeLabels(_ annotations: some Collection>) throws -> (labels: [String?], encoded: [Int])
```

## See Also

### Encoding and decoding the classifier

func encode(TreeClassifierModel&lt;Label>, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> TreeClassifierModel&lt;Label>

Decodes a previously fitted transformer.

