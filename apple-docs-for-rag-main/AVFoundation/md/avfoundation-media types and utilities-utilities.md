

- AVFoundation
-  Media types and utilities 

API Collection

# Media types and utilities

Identify the types of content and file formats that AVFoundation supports.

## Topics

### Media types

struct AVMediaType

An identifier for various media types.

struct AVMediaCharacteristic

A structure that defines media data characteristics.

### File types

struct AVFileType

The uniform type identifiers for various file formats.

struct AVFileTypeProfile

File type profiles for streaming formats.

### Utilities

func AVMakeRect(aspectRatio: CGSize, insideRect: CGRect) -> CGRect

Returns a scaled rectangle that maintains the specified aspect ratio within a bounding rectangle.

## See Also

### Common

Media assets

Load media assets from files and streams to inspect their attributes, tracks, and embedded metadata.

Media reading and writing

Read images from video, export to alternative formats, and perform sample-level reading and writing of media data.

Video settings

Configure video processing settings using standard key and value constants.

Audio settings

Configure audio processing settings using standard key and value constants.

