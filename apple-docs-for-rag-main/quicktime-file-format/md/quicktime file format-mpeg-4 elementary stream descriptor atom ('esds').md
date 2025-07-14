

- QuickTime File Format
-  MPEG-4 elementary stream descriptor atom ('esds') 

Atom

# MPEG-4 elementary stream descriptor atom ('esds')

A required extension to the video sample description for MPEG-4 video.

## Mentioned in 

QuickTime File Format change log

Video sample data

## Overview

This atom contains an MPEG-4 elementary stream descriptor atom. This is a required extension to the video sample description for MPEG-4 video. This extension appears in video sample descriptions only when the codec type is `'mp4v'`.

Note

The elementary stream descriptor which this atom contains is defined in the MPEG-4 specification ISO/IEC FDIS 14496-1.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the elementary stream descriptor atom.

Type

An unsigned 32-bit field.

Version

An unsigned 8-bit integer set to zero.

Flags

A 24-bit field reserved for flags, currently set to zero.

Elementary stream descriptor

An elementary stream descriptor for MPEG-4 video.

## See Also

### Extending video sample descriptions

Pixel aspect ratio ('pasp')

An extension that specifies the height-to-width ratio of pixels found in the video sample.

AVC decoder configuration atom ('avcC')

A required extension to the video sample description for H.264 video.

Color parameter atom ('colr')

A required extension for uncompressed Y´CbCr data formats.

Clean aperture ('clap')

An extension that defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed.

