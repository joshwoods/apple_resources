

- App Intents
- AssistantSchemas
-  AssistantSchemas.SpreadsheetIntent 

Protocol

# AssistantSchemas.SpreadsheetIntent

Assistant schema conformance for app intents that offer spreadsheet functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol SpreadsheetIntent : AssistantSchemas.Model
```

## Mentioned in 

Making spreadsheet actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var addAudioToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding audio to a slide.

var addCommentToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a comment to a sheet in a spreadsheet.

var addImageToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding an image to a sheet in a spreadsheet.

var addTextBoxToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a textbox to a sheet in a spreadsheet.

var addVideoToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a video to a sheet in a spreadsheet.

var addWebVideoToSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a web video to a sheet in a spreadsheet.

var create: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a spreadsheet.

var createSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a sheet in a spreadsheet.

var delete: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a spreadsheet.

var deleteSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a sheet in a spreadsheet.

var open: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a spreadsheet.

var openSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a sheet in a spreadsheet.

var update: some AssistantSchemas.Intent

The app intent conforms to the schema for updating a spreadsheet.

var updateSheet: some AssistantSchemas.Intent

The app intent conforms to the schema for updating a sheet in a spreadsheet.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Spreadsheets

Making spreadsheet actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s spreadsheet functionality with Siri and Apple Intelligence.

protocol SpreadsheetEntity

Assistant schema conformance for app entities that describe spreadsheet data.

