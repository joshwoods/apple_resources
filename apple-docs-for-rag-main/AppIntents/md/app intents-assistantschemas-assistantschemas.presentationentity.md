

- App Intents
- AssistantSchemas
-  AssistantSchemas.PresentationEntity 

Protocol

# AssistantSchemas.PresentationEntity

Assistant schema conformance for app entities that describe presentation data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PresentationEntity : AssistantSchemas.Model
```

## Mentioned in 

Making presentation actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var document: some AssistantSchemas.Entity

The app entity describes a presentation.

var slide: some AssistantSchemas.Entity

The app entity describes a slide.

var template: some AssistantSchemas.Entity

The app entity describes a template for a presentation.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Presentations

Making presentation actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s presentation functionality with Siri and Apple Intelligence.

protocol PresentationIntent

Assistant schema conformance for app intents that offer presentation functionality.

