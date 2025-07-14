

- Media Library
-  MLMediaObjectSampleRateKey 

Global Variable

# MLMediaObjectSampleRateKey

Specifies the media object’s sample rate, in samples per second (Hz). The value for this key is a number (NSNumber).

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
let MLMediaObjectSampleRateKey: String
```

## See Also

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

