

- App Intents
- AssistantSchemas
-  AssistantSchemas.PhotosEntity 

Protocol

# AssistantSchemas.PhotosEntity

Assistant schema conformance for app entities that describe media assets.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PhotosEntity : AssistantSchemas.Model
```

## Mentioned in 

Making photo and video actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var album: some AssistantSchemas.Entity

The app entity describes an album.

var asset: some AssistantSchemas.Entity

The app entity describes a media asset.

var recognizedPerson: some AssistantSchemas.Entity

The app entity describes a person who appears in an asset.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Photos and videos

Making photo and video actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s photo and video functionality with Siri and Apple Intelligence.

protocol PhotosIntent

Assistant schema conformance for app intents that offer photo and video functionality.

protocol PhotosEnum

Assistant schema conformance for types you use to describe photos and videos.

