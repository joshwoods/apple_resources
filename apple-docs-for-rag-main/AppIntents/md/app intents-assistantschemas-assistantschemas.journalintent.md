

- App Intents
- AssistantSchemas
-  AssistantSchemas.JournalIntent 

Protocol

# AssistantSchemas.JournalIntent

Assistant schema conformance for app intents that offer journaling functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol JournalIntent : AssistantSchemas.Model
```

## Mentioned in 

Making journaling actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var createAudioEntry: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a voice journal entry.

var createEntry: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a journal entry.

var deleteEntry: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a journal entry.

var search: some AssistantSchemas.Intent

The app intent conforms to the schema for searching in journal entries.

var updateEntry: some AssistantSchemas.Intent

The app intent conforms to the schema for updating a journal entry.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Journaling

Making journaling actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s journaling functionality with Siri and Apple Intelligence.

protocol JournalEntity

Assistant schema conformance for app entities that describe journaling data.

