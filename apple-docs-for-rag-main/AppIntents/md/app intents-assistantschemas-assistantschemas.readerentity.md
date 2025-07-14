

- App Intents
- AssistantSchemas
-  AssistantSchemas.ReaderEntity 

Protocol

# AssistantSchemas.ReaderEntity

Assistant schema conformance for app entities that describe documents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ReaderEntity : AssistantSchemas.Model
```

## Mentioned in 

Making document reader actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var document: some AssistantSchemas.Entity

The app entity describes a document.

var page: some AssistantSchemas.Entity

The app entity describes a page.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Document reader

Making document reader actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s document viewing and editing functionality with Siri and Apple Intelligence.

protocol ReaderIntent

Assistant schema conformance for app intents that offer document viewing and editing functionality.

protocol ReaderEnum

Assistant schema conformance for types you use to describe documents.

