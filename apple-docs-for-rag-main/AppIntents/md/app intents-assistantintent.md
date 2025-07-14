

- App Intents
-  AssistantIntent 

Protocol

# AssistantIntent

An app intent that Siri performs to fulfill a person’s request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol AssistantIntent : AppIntent
```

## Overview

Don’t adopt this protocol directly, instead use the AssistantIntent(schema:) macro to meet requirements for making your AppIntent available to Siri.

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

### Inherited By

- AssistantSchemaIntent

## See Also

### Base protocols

protocol AssistantSchemaIntent

protocol AssistantEntity

An app entity that Siri can access to fulfill a person’s request.

protocol AssistantSchemaEntity

protocol AssistantEnum

A value that Siri uses to fulfill a person’s request.

protocol AssistantSchemaEnum

