

- App Intents
- AssistantSchemas
-  AssistantSchemas.SystemIntent 

Protocol

# AssistantSchemas.SystemIntent

Assistant schema conformance for app intents that match system-provided intents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol SystemIntent : AssistantSchemas.Model
```

## Topics

### Instance Properties

var search: some AssistantSchemas.Intent

The app intent conforms to the schema for search functionality.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### System and in-app search

Making in-app search actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s search functionality with Siri and Apple Intelligence.

