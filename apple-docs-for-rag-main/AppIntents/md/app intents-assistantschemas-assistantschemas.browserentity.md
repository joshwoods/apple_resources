

- App Intents
- AssistantSchemas
-  AssistantSchemas.BrowserEntity 

Protocol

# AssistantSchemas.BrowserEntity

Assistant schema conformance for app entities that describe data for web browsing functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol BrowserEntity : AssistantSchemas.Model
```

## Mentioned in 

Making browser actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var bookmark: some AssistantSchemas.Entity

The app entity describes a bookmark.

var tab: some AssistantSchemas.Entity

The app entity describes a browser tab.

var window: some AssistantSchemas.Entity

The app entity describes a browser window.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Browser

Making browser actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s web browsing functionality with Siri and Apple Intelligence.

protocol BrowserIntent

Assistant schema conformance for app intents that offer web browsing functionality.

protocol BrowserEnum

Assistant schema conformance for types you use for web browsing functionality.

