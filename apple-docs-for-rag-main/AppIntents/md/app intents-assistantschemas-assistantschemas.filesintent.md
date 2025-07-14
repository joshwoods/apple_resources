

- App Intents
- AssistantSchemas
-  AssistantSchemas.FilesIntent 

Protocol

# AssistantSchemas.FilesIntent

Assistant schema conformance for app intents that offer file management functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol FilesIntent : AssistantSchemas.Model
```

## Mentioned in 

Making file management actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var createFolder: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a folder.

var deleteFiles: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting files.

var moveFiles: some AssistantSchemas.Intent

The app intent conforms to the schema for moving a file.

var openFile: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a file.

var renameFile: some AssistantSchemas.Intent

The app intent conforms to the schema for renaming a file.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### File management

Making file management actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s file management functionality with Siri and Apple Intelligence.

protocol FilesEntity

Assistant schema conformance for app entities that describe files.

