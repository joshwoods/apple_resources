

- Core ML
- MLModelDescription
-  metadata 

Instance Property

# metadata

A dictionary of the model’s creation information, such as its description, author, version, and license.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var metadata: [MLModelMetadataKey : Any] { get }
```

## Discussion

Use the keys defined by MLModelMetadataKey to retrieve the dictionary’s entries.

## See Also

### Accessing Metadata

var classLabels: [Any]?

An array of labels, which can be either strings or a numbers, for classifier models.

struct MLModelMetadataKey

The set of keys the model uses to store values in its metadata dictionary.

