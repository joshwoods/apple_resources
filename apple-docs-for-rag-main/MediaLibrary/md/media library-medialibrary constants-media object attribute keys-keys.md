

- Media Library
- MediaLibrary Constants
-  Media Object Attribute Keys 

API Collection

# Media Object Attribute Keys

Attribute keys for a media object. These constants are used to specify keys within a media object’s attributes dictionary.

## Topics

### Constants

let MLMediaObjectDurationKey: String

Specifies the media object’s duration, in seconds. The value for this key is a number (NSNumber).

let MLMediaObjectArtistKey: String

Specifies the media object’s artist. The value for this key is a string (NSString).

let MLMediaObjectAlbumKey: String

Specifies the media object’s album. The value for this key is a string (NSString).

let MLMediaObjectGenreKey: String

Specifies the media object’s genre. The value for this key is a string (NSString).

let MLMediaObjectKindKey: String

Used by iTunes only. Specifies the media object’s file format (shown in the “Kind” column in iTunes). The value for this key is a string (NSString).

let MLMediaObjectTrackNumberKey: String

Specifies the media object’s track number. The value for this key is a number (NSNumber).

let MLMediaObjectBitRateKey: String

Specifies the media object’s bit rate, in kilobits per second. The value for this key is a number (NSNumber).

let MLMediaObjectSampleRateKey: String

Specifies the media object’s sample rate, in samples per second (Hz). The value for this key is a number (NSNumber).

let MLMediaObjectChannelCountKey: String

Specifies the media object’s channel count. The value for this key is a number (NSNumber).

let MLMediaObjectResolutionStringKey: String

Specifies the media object’s resolution. The value for this key is a string (NSString) intended to be converted to a size (NSSize) using the NSSizeFromString(_:) method.

let MLMediaObjectCommentsKey: String

Specifies the contents of the comments field associated with the media object. The value for this key is a string (NSString).

let MLMediaObjectKeywordsKey: String

Specifies the keywords associated with the media object. The value for this key is an array (NSArray) of strings (NSString).

let MLMediaObjectProtectedKey: String

Specifies whether the media object is protected by DRM (Digital Rights Management). The value for this key is a number (NSNumber), 0 or 1, that represents a Boolean value.

## See Also

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

