

- App Intents
- AssistantSchemas
-  AssistantSchemas.ReaderEnum 

Protocol

# AssistantSchemas.ReaderEnum

Assistant schema conformance for types you use to describe documents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ReaderEnum : AssistantSchemas.Model
```

## Mentioned in 

Making document reader actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var documentKind: some AssistantSchemas.Enum

The file type for a document.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EnumSchema
- AssistantSchemas.EnumSchema

## See Also

### Document reader

Making document reader actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s document viewing and editing functionality with Siri and Apple Intelligence.

protocol ReaderIntent

Assistant schema conformance for app intents that offer document viewing and editing functionality.

protocol ReaderEntity

Assistant schema conformance for app entities that describe documents.

