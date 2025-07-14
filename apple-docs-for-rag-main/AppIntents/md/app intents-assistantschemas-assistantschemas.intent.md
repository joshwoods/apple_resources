

- App Intents
- AssistantSchemas
-  AssistantSchemas.Intent 

Protocol

# AssistantSchemas.Intent

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol Intent : AssistantSchemas.Model
```

## Topics

### Type Properties

static var books: some AssistantSchemas.BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook viewing and rendering functionality.

static var browser: some AssistantSchemas.BrowserIntent

Assistant schema conformance for app intents that offer web browsing functionality.

static var camera: some AssistantSchemas.CameraIntent

Assistant schema conformance for app intents that offer camera functionality.

static var files: some AssistantSchemas.FilesIntent

Assistant schema conformance for app intents that offer file management functionality.

static var journal: some AssistantSchemas.JournalIntent

Assistant schema conformance for app intents that offer journaling functionality.

static var mail: some AssistantSchemas.MailIntent

Assistant schema conformance for app intents that offer email functionality.

static var photos: some AssistantSchemas.PhotosIntent

Assistant schema conformance for app intents that offer photo and video functionality.

static var presentation: some AssistantSchemas.PresentationIntent

static var reader: some AssistantSchemas.ReaderIntent

Assistant schema conformance for app intents that offer document viewing and editing functionality.

static var spreadsheet: some AssistantSchemas.SpreadsheetIntent

Assistant schema conformance for app intents that offer spreadsheet functionality.

static var system: some AssistantSchemas.SystemIntent

Assistant schema conformance for app intents that match system-provided intents.

static var whiteboard: some AssistantSchemas.WhiteboardIntent

Assistant schema conformance for app intents that offer whiteboard functionality.

static var wordProcessor: some AssistantSchemas.WordProcessorIntent

Assistant schema conformance for app intents that offer word processing functionality.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

