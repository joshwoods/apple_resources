

- App Intents
- AssistantSchemas
-  AssistantSchemas.PhotosEnum 

Protocol

# AssistantSchemas.PhotosEnum

Assistant schema conformance for types you use to describe photos and videos.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PhotosEnum : AssistantSchemas.Model
```

## Mentioned in 

Making photo and video actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var albumType: some AssistantSchemas.Enum

The type of photo album.

var assetType: some AssistantSchemas.Enum

The type of asset.

var filterType: some AssistantSchemas.Enum

The filter effect for a photo or video.

var rotationDirection: some AssistantSchemas.Enum

The direction for rotating a photo or video.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EnumSchema
- AssistantSchemas.EnumSchema

## See Also

### Photos and videos

Making photo and video actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s photo and video functionality with Siri and Apple Intelligence.

protocol PhotosIntent

Assistant schema conformance for app intents that offer photo and video functionality.

protocol PhotosEntity

Assistant schema conformance for app entities that describe media assets.

