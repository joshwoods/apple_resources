

- App Intents
- AssistantSchemas
-  AssistantSchemas.WordProcessorIntent 

Protocol

# AssistantSchemas.WordProcessorIntent

Assistant schema conformance for app intents that offer word processing functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol WordProcessorIntent : AssistantSchemas.Model
```

## Mentioned in 

Making word processor actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var addAudioToPage: some AssistantSchemas.Intent

The app intent conforms to the schema for adding audio to a page in a text document.

var addImageToPage: some AssistantSchemas.Intent

The app intent conforms to the schema for adding an image to a page in a text document.

var addTextBoxToPage: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a text box to a page in a text document.

var addVideoToPage: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a video to a page in a text document.

var addWebVideoToPage: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a web video to a page in a text document.

var create: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a text document.

var createPage: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a page in a text document.

var open: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a text document.

var openPage: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a page in a text document.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Word processor and text editing

Making word processor actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s word processor functionality available to Siri and Apple Intelligence.

protocol WordProcessorEntity

Assistant schema conformance for app entities that describe text documents.

