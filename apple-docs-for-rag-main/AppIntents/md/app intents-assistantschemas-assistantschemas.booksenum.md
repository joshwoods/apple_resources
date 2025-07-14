

- App Intents
- AssistantSchemas
-  AssistantSchemas.BooksEnum 

Protocol

# AssistantSchemas.BooksEnum

Assistant schema conformance for types you use to describe ebooks or audiobooks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol BooksEnum : AssistantSchemas.Model
```

## Mentioned in 

Making ebook actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var contentType: some AssistantSchemas.Enum

The content type.

var font: some AssistantSchemas.Enum

The font for rendering a book.

var fontSize: some AssistantSchemas.Enum

The font size for rendering a book.

var navigationDirection: some AssistantSchemas.Enum

The navigation direction of a book.

var pageNavigationSetting: some AssistantSchemas.Enum

Navigation settings for rendering a book.

var relativeCharacterSpacingChange: some AssistantSchemas.Enum

The relative change in character spacing for rendering a book.

var relativeFontChange: some AssistantSchemas.Enum

The relative change of the font for rendering a book.

var relativeLineSpacingChange: some AssistantSchemas.Enum

The relative change in line spacing for rendering a book.

var relativeWordSpacingChange: some AssistantSchemas.Enum

The relative change in word spacing for rendering a book.

var theme: some AssistantSchemas.Enum

The theme for rendering a book.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EnumSchema
- AssistantSchemas.EnumSchema

## See Also

### Books

Making ebook actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s ebook and audiobook functionality with Siri and Apple Intelligence.

protocol BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook functionality.

protocol BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

