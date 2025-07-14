

- App Intents
- AssistantSchemas
-  AssistantSchemas.BrowserIntent 

Protocol

# AssistantSchemas.BrowserIntent

Assistant schema conformance for app intents that offer web browsing functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol BrowserIntent : AssistantSchemas.Model
```

## Mentioned in 

Making browser actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var bookmarkTab: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a new bookmark for a browser tab.

var bookmarkURL: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a bookmark for a URL.

var clearHistory: some AssistantSchemas.Intent

The app intent conforms to the schema for clearing the browser history.

var closeTabs: some AssistantSchemas.Intent

The app intent conforms to the schema for closing a browser tab.

var closeWindows: some AssistantSchemas.Intent

The app intent conforms to the schema for closing one or more browser windows.

var createTab: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a browser tab.

var createWindow: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a new browser window.

var deleteBookmarks: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a bookmark.

var findOnPage: some AssistantSchemas.Intent

The app intent conforms to the schema for finding text on a web page.

var openBookmark: some AssistantSchemas.Intent

The app intent conforms to the Assistant schema for opening a bookmarked URL.

var openURLInTab: some AssistantSchemas.Intent

The app intent conforms to the Assistant schema for loading a URL in a browser tab.

var search: some AssistantSchemas.Intent

The app intent conforms to the Assistant schema for performing a web search.

var switchTab: some AssistantSchemas.Intent

The app intent conforms to the schema for switching to a specific tab.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Browser

Making browser actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s web browsing functionality with Siri and Apple Intelligence.

protocol BrowserEntity

Assistant schema conformance for app entities that describe data for web browsing functionality.

protocol BrowserEnum

Assistant schema conformance for types you use for web browsing functionality.

