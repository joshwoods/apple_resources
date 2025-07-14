

- SwiftData
- Schema
- Schema.Attribute
-  Schema.Attribute.Option 

Structure

# Schema.Attribute.Option

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct Option
```

## Topics

### Accessing property options

static var allowsCloudEncryption: Schema.Attribute.Option

Stores the property’s value in an encrypted form.

static var externalStorage: Schema.Attribute.Option

Stores the property’s value as binary data adjacent to the model storage.

static var preserveValueOnDeletion: Schema.Attribute.Option

Preserves the property’s value in the persistent history when the context deletes the owning model.

static var spotlight: Schema.Attribute.Option

Indexes the property’s value so it can appear in Spotlight search results.

static var unique: Schema.Attribute.Option

Ensures the property’s value is unique across all models of the same type.

static func transformable(by: ValueTransformer.Type) -> Schema.Attribute.Option

Transforms the property’s value between an in-memory form and a persisted form.

static func transformable(by: String) -> Schema.Attribute.Option

### Type Properties

static var ephemeral: Schema.Attribute.Option

Track changes to this property but do not persist

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable

