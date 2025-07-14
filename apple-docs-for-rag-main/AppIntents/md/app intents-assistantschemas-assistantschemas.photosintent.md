

- App Intents
- AssistantSchemas
-  AssistantSchemas.PhotosIntent 

Protocol

# AssistantSchemas.PhotosIntent

Assistant schema conformance for app intents that offer photo and video functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PhotosIntent : AssistantSchemas.Model
```

## Mentioned in 

Making photo and video actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var addAssetsToAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for adding an asset to an album.

var cleanupPhoto: some AssistantSchemas.Intent

The app intent conforms to the schema for undoing edits to an asset.

var copyEdits: some AssistantSchemas.Intent

The app intent conforms to the schema for copying edits to an asset.

var createAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for creating an album.

var createAssets: some AssistantSchemas.Intent

The app intent conforms to the schema for creating an asset.

var crop: some AssistantSchemas.Intent

The app intent conforms to the schema for cropping an asset.

var deleteAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting an album.

var deleteAssets: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting an asset.

var duplicateAssets: some AssistantSchemas.Intent

The app intent conforms to the schema for duplicating an asset.

var openAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for opening an album.

var openAsset: some AssistantSchemas.Intent

The app intent conforms to the schema for opening an asset.

var pasteEdits: some AssistantSchemas.Intent

The app intent conforms to the schema for pasting edits to an asset.

var postToSharedAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for posting an asset to a shared album.

var removeAssetsFromAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for removing an asset from an album.

var search: some AssistantSchemas.Intent

The app intent conforms to the schema for searching the content in the media library.

var setDepth: some AssistantSchemas.Intent

The app intent conforms to the schema for setting the aperture of an asset.

var setExposure: some AssistantSchemas.Intent

The app intent conforms to the schema for setting the exposure of an asset.

var setFilter: some AssistantSchemas.Intent

The app intent conforms to the schema for applying a filter to an asset.

var setRotation: some AssistantSchemas.Intent

The app intent conforms to the schema for rotating an asset.

var setSaturation: some AssistantSchemas.Intent

The app intent conforms to the schema for setting the saturation of an asset.

var setWarmth: some AssistantSchemas.Intent

The app intent conforms to the schema for setting the warmth of an asset.

var straighten: some AssistantSchemas.Intent

The app intent conforms to the schema for straightening an asset.

var toggleDepth: some AssistantSchemas.Intent

The app intent conforms to the schema for toggling the depth of an asset.

var toggleSuggestedEdits: some AssistantSchemas.Intent

The app intent conforms to the schema for enhancing an asset.

var updateAlbum: some AssistantSchemas.Intent

The app intent conforms to the schema for updating an album.

var updateAsset: some AssistantSchemas.Intent

The app intent conforms to the schema for updating an asset.

var updateRecognizedPerson: some AssistantSchemas.Intent

The app intent conforms to the schema for updating a recognized person in an asset.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Photos and videos

Making photo and video actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s photo and video functionality with Siri and Apple Intelligence.

protocol PhotosEntity

Assistant schema conformance for app entities that describe media assets.

protocol PhotosEnum

Assistant schema conformance for types you use to describe photos and videos.

