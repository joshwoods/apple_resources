

- QuickTime File Format
-  AVC decoder configuration atom ('avcC') 

Atom

# AVC decoder configuration atom ('avcC')

A required extension to the video sample description for H.264 video.

## Overview

This atom contains an MPEG-4 decoder configuration atom. This is a required extension to the video sample description for H.264 video. This extension appears in video sample descriptions only when the codec type is `‘avc1’`.

Note

The decoder configuration record that this atom contains is defined in the MPEG-4 specification ISO/IEC FDIS 14496-15.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the AVC decoder configuration atom.

Type

An unsigned 32-bit field.

AVC decoder configuration record

A record that configures the AVC decoder.

## See Also

### Extending video sample descriptions

Pixel aspect ratio ('pasp')

An extension that specifies the height-to-width ratio of pixels found in the video sample.

MPEG-4 elementary stream descriptor atom ('esds')

A required extension to the video sample description for MPEG-4 video.

Color parameter atom ('colr')

A required extension for uncompressed Y´CbCr data formats.

Clean aperture ('clap')

An extension that defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed.

