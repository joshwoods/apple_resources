

- QuickTime File Format
- Media data atom types
- Video media
-  Video sample description extensions 

API Collection

# Video sample description extensions

Extend video sample descriptions by appending other atoms.

## Overview

These atoms are placed after the color table, if one is present. These extensions to the sample description may contain display hints for the decompressor or may simply carry additional information associated with the images. The following table lists the currently defined extensions to video sample descriptions.

| Extension type | Description |
|----|----|
| `'gama'` | A 32-bit fixed-point number indicating the gamma level at which the image was captured. The decompressor can use this value to gamma-correct at display time. |
| `'fiel'` | Two 8-bit integers that define field handling. This information is used by applications to modify decompressed image data or by decompressor components to determine field display order. This extension is mandatory for all uncompressed Y´CbCr data formats. The first byte specifies the field count, and may be set to `1` or `2`. A value of `1` is used for progressive-scan images; a value of `2` indicates interlaced images. When the field count is `2`, the second byte specifies the field ordering: which field contains the topmost scan-line, which field should be displayed earliest, and which is stored first in each sample. Each sample consists of two distinct compressed images, each coding one field: the field with the topmost scan-line, T, and the other field, B. The following defines the permitted variants: `0` – There is only one field. `1` – T is displayed earliest, T is stored first in the file. `6` – B is displayed earliest, B is stored first in the file. `9` – B is displayed earliest, T is stored first in the file. `14` – T is displayed earliest, B is stored first in the file. |
| `'mjqt'` | The default quantization table for a Motion-JPEG data stream. |
| `'mjht'` | The default Huffman table for a Motion-JPEG data stream. |
| `'esds'` | An MPEG-4 elementary stream descriptor atom. This extension is required for MPEG-4 video. For details, see MPEG-4 elementary stream descriptor atom ('esds'). |
| `'avcC'` | An H.264 AVCConfigurationBox. This extension is required for H.264 video as defined in ISO/IEC 14496-15. For details, see AVC decoder configuration atom ('avcC'). |
| `'pasp'` | Pixel aspect ratio. This extension is mandatory for video formats that use non-square pixels. For details, see Pixel aspect ratio ('pasp'). |
| `'colr'` | Color parameters—an image description extension required for all uncompressed Y´CbCr video types. For details, see Color parameter atom ('colr'). |
| `'clap'` | Clean aperture—spatial relationship of Y´CbCr components relative to a canonical image center. This allows accurate alignment for compositing of video images captured using different systems. This is a mandatory extension for all uncompressed Y´CbCr data formats. For details, see Clean aperture ('clap'). |

## Topics

### Extending video sample descriptions

Pixel aspect ratio ('pasp')

An extension that specifies the height-to-width ratio of pixels found in the video sample.

MPEG-4 elementary stream descriptor atom ('esds')

A required extension to the video sample description for MPEG-4 video.

AVC decoder configuration atom ('avcC')

A required extension to the video sample description for H.264 video.

Color parameter atom ('colr')

A required extension for uncompressed Y´CbCr data formats.

Clean aperture ('clap')

An extension that defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed.

## See Also

### Storing video data

Video sample description ('stsd')

An atom that contains information that defines how to interpret video media data.

Video sample data

Store video sample data in different formats, depending on the type of compression you use.

