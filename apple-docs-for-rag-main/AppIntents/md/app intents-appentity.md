

- App Intents
-  AppEntity 

Protocol

# AppEntity

An interface for exposing a custom type or app-specific concept to system experiences like Siri and the Shortcuts app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol AppEntity : AppValue, DisplayRepresentable, Identifiable where Self == Self.ValueType, Self.ID : EntityIdentifierConvertible, Self.ID : Sendable
```

## Mentioned in 

Integrating actions with Siri and Apple Intelligence

Integrating custom data types into your intents

Adding parameters to an app intent

Responding to the Action button on Apple Watch Ultra

## Overview

To use a data model object to app intents, update it to conform to the `AppEntity` protocol. Declare two static properties to make them visible to the system. The following example shows a data model for soup:

For example:

```
struct Soup: AppEntity {
   let id: String

   @Property(title: "Type of soup")
   let type: SoupType = .miso
}
```

For additional types, see EntityProperty.

It is up to you whether you want to conform to the `AppEntity` protocol directly on the data models of your app, or if you create data models specific to your app intents implementation. In many cases, it’s a good idea to create models specific to app intents that shadow your app data models to keep entities separate from the rest of your app’s logic.

## Topics

### Specifying properties

typealias Property

### Making the entity queryable

static var defaultQuery: Self.DefaultQuery

The default query to use to retrieve entity property instances.

**Required** Default implementations provided.

associatedtype DefaultQuery : EntityQuery

**Required**

static var defaultResolverSpecification: EmptyResolverSpecification&lt;Self>

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

Identifiable Implementations

## Relationships

### Inherits From

- AppValue
- CustomLocalizedStringResourceConvertible
- DisplayRepresentable
- Identifiable
- InstanceDisplayRepresentable
- PersistentlyIdentifiable
- Sendable
- TypeDisplayRepresentable

### Inherited By

- AssistantEntity
- AssistantSchemaEntity
- FileEntity
- IndexedEntity
- TransientAppEntity
- URLRepresentableEntity
- UniqueAppEntity

## See Also

### Entities

Integrating custom data types into your intents

Provide the system with information about the types your app uses to model its data so that your intents can use those types as parameters.

protocol FileEntity

An entity that refers to a document or other file.

protocol IndexedEntity

`IndexedEntity` represents an App Entity decorated with an attribute set. A set of attributes that enable the system to perform structured indexing and queries of entities.

protocol TransientAppEntity

A type that represents a transient model object which exposes its interface to App Intents via properties. Note that `TransientAppEntity` types are not meant to be queried.

protocol UniqueAppEntity

An entity that will only ever have one value, such as global settings.

protocol URLRepresentableEntity

An app entity with a URL representation.

