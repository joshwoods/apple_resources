

- Media Library
-  MediaLibrary Constants 

API Collection

# MediaLibrary Constants

## Topics

### Constants

Aperture Media Group Type Identifiers

Identifiers for media group types in the Aperture media source. These constants are used to specify a media group’s typeIdentifier attribute.

Final Cut Pro Media Group Type Identifiers

Identifiers for media group types in the Final Cut Pro media source. These constants are used to specify a media group’s typeIdentifier attribute.

Folders Media Group Type Identifiers

Identifiers for media group types in folder-based media sources. These constants are used to specify a media group’s typeIdentifier attribute.

GarageBand Media Group Type Identifiers

Identifiers for media group types in the GarageBand media source. These constants are used to specify a media group’s typeIdentifier attribute.

Logic Media Group Type Identifiers

Identifiers for media group types in the Logic media source. These constants are used to specify a media group’s typeIdentifier attribute.

let MLMediaLoadAppFoldersKey: String

Specifies one or more relative paths inside the caller’s app bundle in which to search for media files. The value for this key is an array of strings (relative paths inside the caller’s app bundle).

let MLMediaLoadAppleLoops: String

Identifies the folder containing audio loops from Apple.

let MLMediaLoadExcludeSourcesKey: String

Defines which media sources to exclude when loading. This option is processed after MLMediaLoadIncludeSourcesKey. The value for this key is an array of strings (media source identifiers). For a list of valid media source identifiers, see Media Source Identifiers.

let MLMediaLoadFoldersKey: String

Specifies the well-known folders that should be searched for media files. If this key is not present, none of the well-known folders will be provided. The value for this key is an array of strings (identifiers that correspond to well-known folder locations). For a list of well-known folder identifiers, see Well-Known Folder Identifiers.

let MLMediaLoadIncludeSourcesKey: String

Defines which media sources to include when loading. If not present, load all available media sources. This option is processed after MLMediaLoadSourceTypesKey. If MLMediaLoadIncludeSourcesKey is present but MLMediaLoadSourceTypesKey is not, then only those sources specified here will be loaded. This is useful for loading a single media source. When both keys are present, this is useful for adding one or more media sources that normally would not appear for the requested library type. The value for this key is an array of strings (media source identifiers). For a list of valid media source identifiers, see Media Source Identifiers.

let MLMediaLoadMoviesFolder: String

Identifies the user’s Movies folder.

let MLMediaLoadSourceTypesKey: String

Defines which sources to load based on library type. If not present, this will load all sources. The value for this key is a media source type. For a list of valid media source types, see MLMediaSourceType.

let MLMediaSourceApertureIdentifier: String

The media source providing content from Aperture.

let MLMediaSourceAppDefinedFoldersIdentifier: String

The media source for app-defined folders. This identifies a media source created from a relative path inside the caller’s app bundle. This source provides data when MLMediaLoadAppFoldersKey is provided in the options.

let MLMediaSourceCustomFoldersIdentifier: String

The media source for custom folders. Currently, the only custom folder is the folder containing audio loops from Apple. This source provides data when MLMediaLoadFoldersKey is provided with the MLMediaLoadAppleLoops value.

let MLMediaSourceFinalCutIdentifier: String

The media source providing content from Final Cut Pro.

let MLMediaSourceGarageBandIdentifier: String

The media source providing content from GarageBand.

let MLMediaSourceLogicIdentifier: String

The media source providing content from Logic.

let MLMediaSourceMoviesFolderIdentifier: String

The media source for the user’s Movies folder. This source provides data when MLMediaLoadFoldersKey is provided with the MLMediaLoadMoviesFolder value.

let MLMediaSourcePhotoBoothIdentifier: String

The media source providing content from Photo Booth.

let MLMediaSourcePhotosIdentifier: String

struct MLMediaSourceType

Specifies the source type associated with a particular media source. Source type reflects the primary type of media within the source. These constants are used to specify values for MLMediaLoadSourceTypesKey in the init(options:) method of MLMediaLibrary.

let MLMediaSourceiMovieIdentifier: String

The media source providing content from iMovie.

let MLMediaSourceiPhotoIdentifier: String

The media source providing content from iPhoto.

let MLMediaSourceiTunesIdentifier: String

The media source providing content from iTunes.

enum MLMediaType

Specifies the media type associated with a particular media object. These constants are used to specify a media object’s mediaType attribute.

let MLPhotosAlbumTypeIdentifier: String

let MLPhotosAlbumsGroupTypeIdentifier: String

let MLPhotosAllCollectionsGroupTypeIdentifier: String

let MLPhotosAllMomentsGroupTypeIdentifier: String

let MLPhotosAllPhotosAlbumTypeIdentifier: String

let MLPhotosAllYearsGroupTypeIdentifier: String

let MLPhotosBurstGroupTypeIdentifier: String

let MLPhotosCollectionGroupTypeIdentifier: String

let MLPhotosDepthEffectGroupTypeIdentifier: String

let MLPhotosFacesAlbumTypeIdentifier: String

let MLPhotosFavoritesGroupTypeIdentifier: String

let MLPhotosFolderTypeIdentifier: String

let MLPhotosFrontCameraGroupTypeIdentifier: String

let MLPhotosLastImportGroupTypeIdentifier: String

let MLPhotosMomentGroupTypeIdentifier: String

let MLPhotosMyPhotoStreamTypeIdentifier: String

let MLPhotosPanoramasGroupTypeIdentifier: String

let MLPhotosPublishedAlbumTypeIdentifier: String

let MLPhotosRootGroupTypeIdentifier: String

let MLPhotosScreenshotGroupTypeIdentifier: String

let MLPhotosSharedGroupTypeIdentifier: String

let MLPhotosSharedPhotoStreamTypeIdentifier: String

let MLPhotosSloMoGroupTypeIdentifier: String

let MLPhotosSmartAlbumTypeIdentifier: String

let MLPhotosTimelapseGroupTypeIdentifier: String

let MLPhotosVideosGroupTypeIdentifier: String

let MLPhotosYearGroupTypeIdentifier: String

let MLiTunesMusicVideosPlaylistTypeIdentifier: String

let MLiTunesVideoPlaylistTypeIdentifier: String

Media Object Attribute Keys

Attribute keys for a media object. These constants are used to specify keys within a media object’s attributes dictionary.

iMovie Media Group Type Identifiers

Identifiers for media group types in the iMovie media source. These constants are used to specify a media group’s typeIdentifier attribute.

iPhoto Media Group Type Identifiers

Identifiers for media group types in the iPhoto media source. These constants are used to specify a media group’s typeIdentifier attribute.

iTunes Media Group Type Identifiers

Identifiers for media group types in the iTunes media source. These constants are used to specify a media group’s typeIdentifier attribute.

let MLPhotosAnimatedGroupTypeIdentifier: String

let MLPhotosLivePhotosGroupTypeIdentifier: String

let MLPhotosLongExposureGroupTypeIdentifier: String

