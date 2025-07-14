

- Core ML
- MLModelDescription
-  classLabels 

Instance Property

# classLabels

An array of labels, which can be either strings or a numbers, for classifier models.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var classLabels: [Any]? { get }
```

## See Also

### Accessing Metadata

var metadata: [MLModelMetadataKey : Any]

A dictionary of the model’s creation information, such as its description, author, version, and license.

struct MLModelMetadataKey

The set of keys the model uses to store values in its metadata dictionary.

