

- Media Library
-  MLMediaLibrary 

Class

# MLMediaLibrary

The `MLMediaLibrary` class provides an interface for accessing a collection of media objects from various sources. It serves as the initial access point of the Media Library framework.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
class MLMediaLibrary
```

## Overview

The media library structure is defined by MLMediaSource, MLMediaGroup, and MLMediaObject classes. At the highest level, all content within a media library instance is categorized by media source. Conceptually, a media source represents a single app, such as iTunes or Aperture. Each source contains a hierarchy of media groups that originates from a root group. These groups consist of media objects—individual files containing a piece of media such as a photo, song, or movie. Only one copy of each object exists within a media library instance, but an object can be referenced by multiple groups from a single source. The structure of the group hierarchy is specific to each media source.

A media library is initialized using the init(options:) method. The options argument to this method serves as a filter. By specifying which folders or sources to include or exclude during load, you can view a particular subset of groups and objects from your collection. All objects provided are thread-safe. For descriptions of possible load options, see Load Options Keys.

The typical and most efficient use case is to create and use one instance of `MLMediaLibrary` for the lifetime of an app. When the underlying media files and metadata on the user’s system change, the corresponding data model objects (media groups and media objects) are automatically updated and KVO notifications are sent to notify the calling code of any changes. Multiple instances of `MLMediaLibrary` can be created and used, but their sources, groups, and objects will be independent of those provided by other instances of `MLMediaLibrary`.

## Topics

### Initializing the Library

init(options: [String : Any])

Initializes the media library based on the specified load options.

### Accessing Media Sources

var mediaSources: [String : MLMediaSource]?

Returns a dictionary of media sources by identifier.

### Constants

Load Options Keys

Keys used to specify the `options` dictionary argument to init(options:).

Media Source Identifiers

Identifiers for media sources which correspond to apps used to manage groups of media objects. Used with Load Options Keys.

Non-App-Specific Media Source Identifiers

Identifiers for media sources which do not correspond to apps. Used with Load Options Keys.

Well-Known Folder Identifiers

Identifiers for well-known media folders used to specify the value for MLMediaLoadFoldersKey.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class MLMediaGroup

The `MLMediaGroup` class provides groupings for media objects from a single source of media, such as iTunes or Aperture. The media objects—individual files containing a piece of media such as a photo, song, or movie—are referenced by one or more groups within each media source. These groupings serve as filters, providing hierarchical structure to the collection of objects in each source.

class MLMediaObject

The `MLMediaObject` class describes a single media file, such as a photo, song, or movie. Each media object contains basic metadata including a name, media type, URL, and so on. Additional information about each object is stored in its list of attributes. For a list of possible object attribute keys, see Media Object Attribute Keys.

class MLMediaSource

The `MLMediaSource` class identifies a specific provider of media. Conceptually, a media source respresents a single app, such as iTunes or Aperture. Each media source contains multiple groups of media objects—individual files containing a piece of media such as a photo, song, or movie.

