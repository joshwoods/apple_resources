

- App Intents
- AssistantSchemas
-  AssistantSchemas.ReaderIntent 

Protocol

# AssistantSchemas.ReaderIntent

Assistant schema conformance for app intents that offer document viewing and editing functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ReaderIntent : AssistantSchemas.Model
```

## Mentioned in 

Making document reader actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var deletePages: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a page.

var enhanceDocuments: some AssistantSchemas.Intent

The app intent conforms to the schema for enhancing a document.

var insertPages: some AssistantSchemas.Intent

The app intent conforms to the schema for inserting a page.

var openDocument: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a text document.

var openPage: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a document.

var resizeDocuments: some AssistantSchemas.Intent

The app intent conforms to the schema for resizing a document.

var rotateDocuments: some AssistantSchemas.Intent

The app intent conforms to the schema for rotating a document.

var rotatePages: some AssistantSchemas.Intent

The app intent conforms to the schema for rotating a page.

var searchDocuments: some AssistantSchemas.Intent

The app intent conforms to the schema for searching in a document.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Document reader

Making document reader actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s document viewing and editing functionality with Siri and Apple Intelligence.

protocol ReaderEntity

Assistant schema conformance for app entities that describe documents.

protocol ReaderEnum

Assistant schema conformance for types you use to describe documents.

