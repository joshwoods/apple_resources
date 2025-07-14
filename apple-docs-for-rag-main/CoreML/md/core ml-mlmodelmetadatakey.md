

- Core ML
-  MLModelMetadataKey 

Structure

# MLModelMetadataKey

The set of keys the model uses to store values in its metadata dictionary.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
struct MLModelMetadataKey
```

## Topics

### Metadata Keys

static let author: MLModelMetadataKey

Key for the author of the model.

static let description: MLModelMetadataKey

Key for the overall description of the model.

static let license: MLModelMetadataKey

Key for the license of the model.

static let versionString: MLModelMetadataKey

Key for the version of the model.

static let creatorDefinedKey: MLModelMetadataKey

Key for the model creator’s custom metadata.

### Creating Metadata

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Metadata

var classLabels: [Any]?

An array of labels, which can be either strings or a numbers, for classifier models.

var metadata: [MLModelMetadataKey : Any]

A dictionary of the model’s creation information, such as its description, author, version, and license.

