

- App Intents
- AssistantSchemas
-  AssistantSchemas.BooksIntent 

Protocol

# AssistantSchemas.BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol BooksIntent : AssistantSchemas.Model
```

## Mentioned in 

Making ebook actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var navigatePage: some AssistantSchemas.Intent

The app intent conforms to the schema for navigating to a specific page of an ebook.

var openBook: some AssistantSchemas.Intent

The app intent conforms to the schema for opening an ebook.

var playAudiobook: some AssistantSchemas.Intent

The app intent conforms to the schema for playing an audiobook.

var search: some AssistantSchemas.Intent

The app intent conforms to the schema for searching an ebook or audiobook library.

var updateCharacterSpacing: some AssistantSchemas.Intent

The app intent conforms to the schema for updating the character spacing.

var updateFontSize: some AssistantSchemas.Intent

The app intent conforms to the schema for updating the font size.

var updateLineSpacing: some AssistantSchemas.Intent

The app intent conforms to the schema for updating the line spacing.

var updateSettings: some AssistantSchemas.Intent

The app intent conforms to the schema for updating settings for an ebook.

var updateWordSpacing: some AssistantSchemas.Intent

The app intent conforms to the schema for updating the spacing between words.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Books

Making ebook actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s ebook and audiobook functionality with Siri and Apple Intelligence.

protocol BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

protocol BooksEnum

Assistant schema conformance for types you use to describe ebooks or audiobooks.

