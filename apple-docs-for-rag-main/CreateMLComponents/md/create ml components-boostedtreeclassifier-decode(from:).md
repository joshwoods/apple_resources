

- Create ML Components
- BoostedTreeClassifier
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> TreeClassifierModel
```

## See Also

### Encoding and decoding the classifier

func encode(TreeClassifierModel&lt;Label>, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func encodeLabels(some Collection&lt;Optional&lt;Label>>) throws -> (labels: [String?], encoded: [Int])

