

- App Intents
-  AssistantEntity 

Protocol

# AssistantEntity

An app entity that Siri can access to fulfill a person’s request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol AssistantEntity : AppEntity
```

## Overview

Don’t adopt this protocol directly, instead use the AssistantEntity(schema:) macro to meet requirements for making your AppEntity available to Siri.

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

### Inherited By

- AssistantSchemaEntity

## See Also

### Base protocols

protocol AssistantIntent

An app intent that Siri performs to fulfill a person’s request.

protocol AssistantSchemaIntent

protocol AssistantSchemaEntity

protocol AssistantEnum

A value that Siri uses to fulfill a person’s request.

protocol AssistantSchemaEnum

