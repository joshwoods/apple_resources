

- Media Library
- MLMediaLibrary
-  Non-App-Specific Media Source Identifiers 

API Collection

# Non-App-Specific Media Source Identifiers

Identifiers for media sources which do not correspond to apps. Used with Load Options Keys.

## Topics

### Constants

let MLMediaSourceMoviesFolderIdentifier: String

The media source for the user’s Movies folder. This source provides data when MLMediaLoadFoldersKey is provided with the MLMediaLoadMoviesFolder value.

let MLMediaSourceCustomFoldersIdentifier: String

The media source for custom folders. Currently, the only custom folder is the folder containing audio loops from Apple. This source provides data when MLMediaLoadFoldersKey is provided with the MLMediaLoadAppleLoops value.

let MLMediaSourceAppDefinedFoldersIdentifier: String

The media source for app-defined folders. This identifies a media source created from a relative path inside the caller’s app bundle. This source provides data when MLMediaLoadAppFoldersKey is provided in the options.

## See Also

### Constants

Load Options Keys

Keys used to specify the `options` dictionary argument to init(options:).

Media Source Identifiers

Identifiers for media sources which correspond to apps used to manage groups of media objects. Used with Load Options Keys.

Well-Known Folder Identifiers

Identifiers for well-known media folders used to specify the value for MLMediaLoadFoldersKey.

