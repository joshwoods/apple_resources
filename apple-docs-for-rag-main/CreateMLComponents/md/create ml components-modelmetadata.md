

- Create ML Components
-  ModelMetadata 

Structure

# ModelMetadata

User info keys that specify useful information about a model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct ModelMetadata
```

## Topics

### Creating a model

init(description: String, version: String, author: String, license: String, creatorDefined: [String : String])

Creates model metadata.

### Getting the properties

var author: String

The author of this model.

var creatorDefined: [String : String]

Creator-defined custom metadata.

var description: String

A short description of what the model does and/or its purpose.

var license: String

License information for the model.

var version: String

A version number encoded as a string.

### Operators

static func == (ModelMetadata, ModelMetadata) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Core ML adaptors

struct MLModelTransformerAdaptor

A transformer that uses a Core ML model.

struct MLModelClassifierAdaptor

A transformer that uses a Core ML model as a classifier.

struct MLModelRegressorAdaptor

A transformer that uses a Core ML model as a regressor.

