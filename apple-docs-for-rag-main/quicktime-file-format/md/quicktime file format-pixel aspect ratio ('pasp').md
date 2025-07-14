

- QuickTime File Format
-  Pixel aspect ratio ('pasp') 

Atom

# Pixel aspect ratio ('pasp')

An extension that specifies the height-to-width ratio of pixels found in the video sample.

## Mentioned in 

Video sample data

QuickTime File Format change log

## Overview

This is a required extension for MPEG-4 and uncompressed Y´CbCr video formats when non-square pixels are used. It is optional when square pixels are used.

The units of measure for the `hSpacing` and `vSpacing` parameters are not specified, as only the ratio matters. The units of measure for height and width must be the same, however.

The following table shows some common pixel aspect ratios.

| Description                               | hSpacing | vSpacing |
|-------------------------------------------|----------|----------|
| 4:3 square pixels (composite NTSC or PAL) | `1`      | `1`      |
| 4:3 non-square 525 (NTSC)                 | `10`     | `11`     |
| 4:3 non-square 625 (PAL)                  | `59`     | `54`     |
| 16:9 analog (composite NTSC or PAL)       | `4`      | `3`      |
| 16:9 digital 525 (NTSC)                   | `40`     | `33`     |
| 16:9 digital 625 (PAL)                    | `118`    | `81`     |
| 1920x1035 HDTV (per SMPTE 260M-1992)      | `113`    | `118`    |
| 1920x1035 HDTV (per SMPTE RP 187-1995)    | `1018`   | `1062`   |
| 1920x1080 HDTV or 1280x720 HDTV           | `1`      | `1`      |

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the pixel aspect ratio atom.

Type

An unsigned 32-bit field.

hSpacing

An unsigned 32-bit integer specifying the horizontal spacing of pixels, such as luma sampling instants for Y´CbCr or YUV video.

vSpacing

An unsigned 32-bit integer specifying the vertical spacing of pixels, such as video picture lines.

## See Also

### Extending video sample descriptions

MPEG-4 elementary stream descriptor atom ('esds')

A required extension to the video sample description for MPEG-4 video.

AVC decoder configuration atom ('avcC')

A required extension to the video sample description for H.264 video.

Color parameter atom ('colr')

A required extension for uncompressed Y´CbCr data formats.

Clean aperture ('clap')

An extension that defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed.

