

- App Intents
- AssistantSchemas
-  AssistantSchemas.BooksEntity 

Protocol

# AssistantSchemas.BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol BooksEntity : AssistantSchemas.Model
```

## Mentioned in 

Making ebook actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var audiobook: some AssistantSchemas.Entity

The app entity describes an audiobook.

var book: some AssistantSchemas.Entity

The app entity describes an ebook.

var settings: some AssistantSchemas.Entity

The app entity describes settings for an audiobook or ebook.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Books

Making ebook actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s ebook and audiobook functionality with Siri and Apple Intelligence.

protocol BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook functionality.

protocol BooksEnum

Assistant schema conformance for types you use to describe ebooks or audiobooks.

