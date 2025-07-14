

- App Intents
- AssistantSchemas
-  AssistantSchemas.PresentationIntent 

Protocol

# AssistantSchemas.PresentationIntent

Assistant schema conformance for app intents that offer presentation functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PresentationIntent : AssistantSchemas.Model
```

## Mentioned in 

Making presentation actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var addAudioToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding audio to a slide.

var addCommentToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a comment to a slide.

var addImageToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding an image to a slide.

var addTextBoxToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a text box to a slide.

var addVideoToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a video to a slide.

var addWebVideoToSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for adding a video from the internet to a slide.

var create: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a presentation.

var createSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for creating a new slide for a presentation.

var deleteSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting a slide.

var open: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a presentation.

var openSlide: some AssistantSchemas.Intent

The app intent conforms to the schema for opening a slide of a presentation.

var setSlideTitle: some AssistantSchemas.Intent

The app intent conforms to the schema for setting the title of a slide.

var startPlayback: some AssistantSchemas.Intent

The app intent conforms to the schema for starting a presentation.

var stopPlayback: some AssistantSchemas.Intent

The app intent conforms to the schema for stopping a presentation.

var update: some AssistantSchemas.Intent

The app intent conforms to the schema for updating the name of a presentation.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Presentations

Making presentation actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s presentation functionality with Siri and Apple Intelligence.

protocol PresentationEntity

Assistant schema conformance for app entities that describe presentation data.

