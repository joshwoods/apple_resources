

- Media Player
- MPMediaItem
-  User-defined property keys 

API Collection

# User-defined property keys

Properties for obtaining user-defined metadata for a media item.

## Overview

Obtain user-defined metadata for a media item by calling the value(forProperty:) method with these property keys. Don’t use user-defined properties to build media property predicates.

## Topics

### User-defined property keys

let MPMediaItemPropertySkipCount: String

The number of times the user has skipped playing the item.

let MPMediaItemPropertyRating: String

The user-specified rating of the object in the range `[0...5]`, where a value of 5 indicates the most favorable rating.

let MPMediaItemPropertyLastPlayedDate: String

The most recent calendar date on which the user played the media item.

let MPMediaItemPropertyUserGrouping: String

Corresponds to the “Grouping” field in the Info tab in the Get Info dialog in iTunes.

let MPMediaItemPropertyBookmarkTime: String

The user’s place in the media item the most recent time it was played.

let MPMediaItemPropertyDateAdded: String

The date the media item was added to the user’s Media library.

## See Also

### Media item types and keys

struct MPMediaType

The properties for defining the type for a media item.

General media item property keys

System-defined properties for obtaining the metadata for a media item.

