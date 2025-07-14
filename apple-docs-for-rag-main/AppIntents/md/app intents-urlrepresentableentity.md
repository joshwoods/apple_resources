

- App Intents
-  URLRepresentableEntity 

Protocol

# URLRepresentableEntity

An app entity with a URL representation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol URLRepresentableEntity : AppEntity, CustomURLRepresentationParameterConvertible
```

## Overview

Add support for `URLRepresentableEntity` to your app entities to add a URL representation. This allows Siri and Shortcuts to treat the entity like a universal link to specific content, allowing actions to open the URL or to make it sharable.

Note that you need to use a universal link for your URL representation, you can’t use a custom URL scheme. For more information about universal links, see Allowing apps and websites to link to your content.

## Topics

### Type Aliases

typealias URLRepresentation

### Type Properties

static var urlRepresentation: Self.URLRepresentation

**Required** Default implementation provided.

## Relationships

### Inherits From

- AppEntity
- AppValue
- CustomLocalizedStringResourceConvertible
- CustomURLRepresentationParameterConvertible
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

protocol FileEntity

An entity that refers to a document or other file.

protocol IndexedEntity

`IndexedEntity` represents an App Entity decorated with an attribute set. A set of attributes that enable the system to perform structured indexing and queries of entities.

protocol TransientAppEntity

A type that represents a transient model object which exposes its interface to App Intents via properties. Note that `TransientAppEntity` types are not meant to be queried.

protocol UniqueAppEntity

An entity that will only ever have one value, such as global settings.

