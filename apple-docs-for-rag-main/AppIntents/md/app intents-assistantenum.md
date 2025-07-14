

- App Intents
-  AssistantEnum 

Protocol

# AssistantEnum

A value that Siri uses to fulfill a person’s request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol AssistantEnum : AppEnum
```

## Overview

Don’t adopt this protocol directly, instead use the AssistantEnum(schema:) macro to meet requirements for making your AppEnum available to Siri.

## Relationships

### Inherits From

- AppEnum
- AppValue
- CaseDisplayRepresentable
- CaseIterable
- CustomLocalizedStringResourceConvertible
- Equatable
- Hashable
- PersistentlyIdentifiable
- RawRepresentable
- Sendable
- StaticDisplayRepresentable
- TypeDisplayRepresentable

### Inherited By

- AssistantSchemaEnum

## See Also

### Base protocols

protocol AssistantIntent

An app intent that Siri performs to fulfill a person’s request.

protocol AssistantSchemaIntent

protocol AssistantEntity

An app entity that Siri can access to fulfill a person’s request.

protocol AssistantSchemaEntity

protocol AssistantSchemaEnum

