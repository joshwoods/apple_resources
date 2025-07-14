

- Media Library
-  MLPhotosLastImportGroupTypeIdentifier 

Global Variable

# MLPhotosLastImportGroupTypeIdentifier

Mac Catalyst 13.0+macOS 10.10–10.15Deprecated

``` source
let MLPhotosLastImportGroupTypeIdentifier: String
```

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

