

- App Intents
- AssistantSchemas
-  AssistantSchemas.Entity 

Protocol

# AssistantSchemas.Entity

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol Entity : AssistantSchemas.Model
```

## Topics

### Type Properties

static var books: some AssistantSchemas.BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

static var browser: some AssistantSchemas.BrowserEntity

The app entity describes a data for web browsing functionality.

static var files: some AssistantSchemas.FilesEntity

Assistant schema conformance for app entities that describe file data.

static var journal: some AssistantSchemas.JournalEntity

Assistant schema conformance for app entities that describe journaling data.

static var mail: some AssistantSchemas.MailEntity

Assistant schema conformance for app entities that describe email data.

static var photos: some AssistantSchemas.PhotosEntity

Assistant schema conformance for app entities that describe media assets.

static var presentation: some AssistantSchemas.PresentationEntity

Assistant schema conformance for app entities that describe presentation data.

static var reader: some AssistantSchemas.ReaderEntity

Assistant schema conformance for app entities that describe media assets.

static var spreadsheet: some AssistantSchemas.SpreadsheetEntity

Assistant schema conformance for app entities that describe spreadsheet data.

static var whiteboard: some AssistantSchemas.WhiteboardEntity

Assistant schema conformance for app entities that describe data for whiteboard functionality.

static var wordProcessor: some AssistantSchemas.WordProcessorEntity

Assistant schema conformance for app entities that describe text document data.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

