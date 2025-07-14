

- App Intents
-  AppValue 

Protocol

# AppValue

An interface that describes conceptual types you use in app intents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol AppValue : PersistentlyIdentifiable, TypeDisplayRepresentable, _IntentValue, Sendable
```

## Overview

This protocol serves as the base type for conceptual interfaces like AppEntity or AppEnum.

## Relationships

### Inherits From

- PersistentlyIdentifiable
- Sendable
- TypeDisplayRepresentable

### Inherited By

- AppEntity
- AppEnum
- AssistantEntity
- AssistantEnum
- AssistantSchemaEntity
- AssistantSchemaEnum
- FileEntity
- IndexedEntity
- TransientAppEntity
- URLRepresentableEntity
- URLRepresentableEnum
- UniqueAppEntity

### Conforming Types

- StringSearchScope
- VideoCategory

## See Also

### Entity content

class EntityProperty

A property wrapper that exposes the associated property to the system.

protocol AnyIntentValue

A type the system uses to access a parameter or property value.

protocol AppEnum

An interface to express that a custom type has a predefined, static set of valid values to display.

protocol URLRepresentableEnum

An app enum with a URL representation.

