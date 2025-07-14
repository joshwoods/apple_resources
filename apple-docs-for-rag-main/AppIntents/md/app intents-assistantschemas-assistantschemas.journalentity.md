

- App Intents
- AssistantSchemas
-  AssistantSchemas.JournalEntity 

Protocol

# AssistantSchemas.JournalEntity

Assistant schema conformance for app entities that describe journaling data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol JournalEntity : AssistantSchemas.Model
```

## Mentioned in 

Making journaling actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var entry: some AssistantSchemas.Entity

The app entity describes a journal entry.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Journaling

Making journaling actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s journaling functionality with Siri and Apple Intelligence.

protocol JournalIntent

Assistant schema conformance for app intents that offer journaling functionality.

