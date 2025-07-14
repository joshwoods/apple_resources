

- App Intents
-  App intent domains 

API Collection

# App intent domains

Make your app’s actions and content available to Siri and Apple Intelligence with assistant schemas.

## Overview

To enable enhanced understanding and more conversational interactions with Siri for your app, choose a domain and a schema that match your app’s functionality. By conforming your app intent, app entity, or your app enumeration to a schema, you ensure that Apple Intelligence understands your app’s actions and content. When you’ve identified the schema to use, leverage the AssistantIntent(schema:), AssistantEntity(schema:), and AssistantEnum(schema:) macros to write schema-conforming code.

To learn more, refer to Integrating actions with Siri and Apple Intelligence and Making onscreen content available to Siri and Apple Intelligence.

## Topics

### Macros

macro AssistantIntent&lt;T>(schema: T)

A Swift macro you use to make sure your app intent conforms to an assistant schema.

macro AssistantEntity&lt;T>(schema: T)

A Swift macro you use to make sure your app entity conforms to an assistant schema.

macro AssistantEnum&lt;T>(schema: T)

A Swift macro you use to make sure your app enum conforms to an assistant schema.

### Books

Making ebook actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s ebook and audiobook functionality with Siri and Apple Intelligence.

protocol BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook functionality.

protocol BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

protocol BooksEnum

Assistant schema conformance for types you use to describe ebooks or audiobooks.

### Browser

Making browser actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s web browsing functionality with Siri and Apple Intelligence.

protocol BrowserIntent

Assistant schema conformance for app intents that offer web browsing functionality.

protocol BrowserEntity

Assistant schema conformance for app entities that describe data for web browsing functionality.

protocol BrowserEnum

Assistant schema conformance for types you use for web browsing functionality.

### Camera

Making camera actions available to Siri and Apple Intelligence

Create app intents and enumerations to integrate your app’s camera functionality with Siri and Apple Intelligence.

protocol CameraIntent

Assistant schema conformance for app intents that offer camera functionality.

protocol CameraEnum

Assistant schema conformance for types you use for camera functionality.

### Document reader

Making document reader actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s document viewing and editing functionality with Siri and Apple Intelligence.

protocol ReaderIntent

Assistant schema conformance for app intents that offer document viewing and editing functionality.

protocol ReaderEntity

Assistant schema conformance for app entities that describe documents.

protocol ReaderEnum

Assistant schema conformance for types you use to describe documents.

### File management

Making file management actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s file management functionality with Siri and Apple Intelligence.

protocol FilesIntent

Assistant schema conformance for app intents that offer file management functionality.

protocol FilesEntity

Assistant schema conformance for app entities that describe files.

### Journaling

Making journaling actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s journaling functionality with Siri and Apple Intelligence.

protocol JournalIntent

Assistant schema conformance for app intents that offer journaling functionality.

protocol JournalEntity

Assistant schema conformance for app entities that describe journaling data.

### Email

Making email actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s email functionality with Siri and Apple Intelligence.

protocol MailIntent

Assistant schema conformance for app intents that offer email functionality.

protocol MailEntity

Assistant schema conformance for app entities that describe email.

### Photos and videos

Making photo and video actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s photo and video functionality with Siri and Apple Intelligence.

protocol PhotosIntent

Assistant schema conformance for app intents that offer photo and video functionality.

protocol PhotosEntity

Assistant schema conformance for app entities that describe media assets.

protocol PhotosEnum

Assistant schema conformance for types you use to describe photos and videos.

### Presentations

Making presentation actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s presentation functionality with Siri and Apple Intelligence.

protocol PresentationIntent

Assistant schema conformance for app intents that offer presentation functionality.

protocol PresentationEntity

Assistant schema conformance for app entities that describe presentation data.

### Spreadsheets

Making spreadsheet actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s spreadsheet functionality with Siri and Apple Intelligence.

protocol SpreadsheetIntent

Assistant schema conformance for app intents that offer spreadsheet functionality.

protocol SpreadsheetEntity

Assistant schema conformance for app entities that describe spreadsheet data.

### System and in-app search

Making in-app search actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s search functionality with Siri and Apple Intelligence.

protocol SystemIntent

Assistant schema conformance for app intents that match system-provided intents.

### Whiteboard

Making whiteboard actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s whiteboard functionality available to Siri and Apple Intelligence.

protocol WhiteboardIntent

Assistant schema conformance for app intents that offer whiteboard functionality.

protocol WhiteboardEntity

Assistant schema conformance for app entities that describe data for whiteboard functionality.

protocol WhiteboardEnum

Assistant schema conformance for whiteboard types.

### Word processor and text editing

Making word processor actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s word processor functionality available to Siri and Apple Intelligence.

protocol WordProcessorIntent

Assistant schema conformance for app intents that offer word processing functionality.

protocol WordProcessorEntity

Assistant schema conformance for app entities that describe text documents.

### Base protocols

Assistant schema base protocols

Protocols that provide the underlying functionality for assistant schemas.

## See Also

### Siri and Apple Intelligence

Integrating actions with Siri and Apple Intelligence

Create app intents, entities, and enumerations that conform to assistant schemas to tap into the enhanced action capabilities of Siri and Apple Intelligence.

Making onscreen content available to Siri and Apple Intelligence

Enable Siri and Apple Intelligence to respond to a person’s questions and action requests for your app’s onscreen content.

Making your app’s functionality available to Siri

Add assistant schemas to your app so Siri can complete requests, and integrate your app with Apple Intelligence, Spotlight, and other system experiences.

