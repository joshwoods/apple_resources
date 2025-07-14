

- App Intents
-  FileEntity 

Protocol

# FileEntity

An entity that refers to a document or other file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol FileEntity : AppEntity where Self.ID == FileEntityIdentifier
```

## Topics

### Type Properties

static var supportedContentTypes: [UTType]

A list of selectable type identifiers. The default value is ‘public.item’.

**Required**

## Relationships

### Inherits From

- AppEntity
- AppValue
- CustomLocalizedStringResourceConvertible
- DisplayRepresentable
- Identifiable
- InstanceDisplayRepresentable
- PersistentlyIdentifiable
- Sendable
- TypeDisplayRepresentable

## See Also

### Entities

Integrating custom data types into your intents

Provide the system with information about the types your app uses to model its data so that your intents can use those types as parameters.

protocol AppEntity

An interface for exposing a custom type or app-specific concept to system experiences like Siri and the Shortcuts app.

protocol IndexedEntity

`IndexedEntity` represents an App Entity decorated with an attribute set. A set of attributes that enable the system to perform structured indexing and queries of entities.

protocol TransientAppEntity

A type that represents a transient model object which exposes its interface to App Intents via properties. Note that `TransientAppEntity` types are not meant to be queried.

protocol UniqueAppEntity

An entity that will only ever have one value, such as global settings.

protocol URLRepresentableEntity

An app entity with a URL representation.

