

- App Intents
- AssistantSchemas
-  AssistantSchemas.WhiteboardIntent 

Protocol

# AssistantSchemas.WhiteboardIntent

Assistant schema conformance for app intents that offer whiteboard functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol WhiteboardIntent : AssistantSchemas.Model
```

## Mentioned in 

Making whiteboard actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var createBoard: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a new whiteboard canvas.

var createItem: some AssistantSchemas.Intent

The app intent conforms to the schema for creating an item on a whiteboard canvas.

var deleteBoard: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a whiteboard canvas.

var deleteItem: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting an item on a whiteboard canvas.

var openBoard: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a new whiteboard canvas.

var updateBoard: some AssistantSchemas.Intent

The app intent conforms to the schema for updating a whiteboard canvas.

var updateItem: some AssistantSchemas.Intent

The app intent conforms to the schema for updating an item on a whiteboard canvas.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Whiteboard

Making whiteboard actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s whiteboard functionality available to Siri and Apple Intelligence.

protocol WhiteboardEntity

Assistant schema conformance for app entities that describe data for whiteboard functionality.

protocol WhiteboardEnum

Assistant schema conformance for whiteboard types.

