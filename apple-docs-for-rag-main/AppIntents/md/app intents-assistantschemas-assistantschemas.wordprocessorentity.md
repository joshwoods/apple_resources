

- App Intents
- AssistantSchemas
-  AssistantSchemas.WordProcessorEntity 

Protocol

# AssistantSchemas.WordProcessorEntity

Assistant schema conformance for app entities that describe text documents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol WordProcessorEntity : AssistantSchemas.Model
```

## Mentioned in 

Making word processor actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var document: some AssistantSchemas.Entity

The app entity describes a text document.

var page: some AssistantSchemas.Entity

The app entity describes a page in a text document.

var template: some AssistantSchemas.Entity

The app entity describes a text document template.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Word processor and text editing

Making word processor actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s word processor functionality available to Siri and Apple Intelligence.

protocol WordProcessorIntent

Assistant schema conformance for app intents that offer word processing functionality.

