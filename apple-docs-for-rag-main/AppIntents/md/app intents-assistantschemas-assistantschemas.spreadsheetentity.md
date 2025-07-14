

- App Intents
- AssistantSchemas
-  AssistantSchemas.SpreadsheetEntity 

Protocol

# AssistantSchemas.SpreadsheetEntity

Assistant schema conformance for app entities that describe spreadsheet data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol SpreadsheetEntity : AssistantSchemas.Model
```

## Mentioned in 

Making spreadsheet actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var document: some AssistantSchemas.Entity

The app entity describes a spreadsheet.

var sheet: some AssistantSchemas.Entity

The app entity describes a sheet in a spreadsheet.

var template: some AssistantSchemas.Entity

The app entity describes a template for a spreadsheet.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Spreadsheets

Making spreadsheet actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s spreadsheet functionality with Siri and Apple Intelligence.

protocol SpreadsheetIntent

Assistant schema conformance for app intents that offer spreadsheet functionality.

