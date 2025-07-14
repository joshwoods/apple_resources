

- QuickTime File Format
-  Video sample description ('stsd') 

Atom

# Video sample description ('stsd')

An atom that contains information that defines how to interpret video media data.

## Overview

The video sample description contains information that defines how to interpret video media data. A video sample description begins with the four fields described in the ‘General structure of a sample description’ section of Sample description atom ('stsd').

Note

Some video sample descriptions contain an optional 4-byte terminator with all bytes set to `0`, following all other sample description and sample description extension data. If this optional terminator is present, the sample description size value will include it. It is important to check the sample description size when parsing: more than or fewer than these four optional bytes, if present in the size value, indicates a malformed sample description.

The data format field of a video sample description indicates the type of compression that was used to compress the image data, or the color space representation of uncompressed video data. The following table shows some of the formats supported. The list is not exhaustive, and is subject to addition.

| Compression type | Description |
|----|----|
| `'cvid'` | Cinepak |
| `'jpeg'` | JPEG |
| `'smc '` | Graphics |
| `'rle '` | Animation |
| `'rpza'` | Apple video |
| `'kpcd'` | Kodak Photo CD |
| `'png '` | Portable Network Graphics |
| `'mjpa'` | Motion-JPEG (format A) |
| `'mjpb'` | Motion-JPEG (format B) |
| `'SVQ1'` | Sorenson video, version 1 |
| `'SVQ3'` | Sorenson video 3 |
| `'mp4v'` | MPEG-4 video |
| `'avc1'` | H.264 video |
| `'dvc '` | NTSC DV-25 video |
| `'dvcp'` | PAL DV-25 video |
| `'gif '` | CompuServe Graphics Interchange Format |
| `'h263'` | H.263 video |
| `'tiff'` | Tagged Image File Format |
| `'raw '` | Uncompressed RGB |
| `'2vuY'` | Uncompressed Y´CbCr, 8-bit-per-component 4:2:2 |
| `'yuv2'` | Uncompressed Y´CbCr, 8-bit-per-component 4:2:2 |
| `'v308'` | Uncompressed Y´CbCr, 8-bit-per-component 4:4:4 |
| `'v408'` | Uncompressed Y´CbCr, 8-bit-per-component 4:4:4:4 |
| `'v216'` | Uncompressed Y´CbCr, 10, 12, 14, or 16-bit-per-component 4:2:2 |
| `'v410'` | Uncompressed Y´CbCr, 10-bit-per-component 4:4:4 |
| `'v210'` | Uncompressed Y´CbCr, 10-bit-per-component 4:2:2 |

## Topics

### Data fields

Sample description size

A 32-bit integer indicating the number of bytes in the sample description.

Data format

A 32-bit integer indicating the format of the stored data.

Reserved

Six bytes.

Data reference index

A 16-bit integer that contains the index of the data reference to use to retrieve data associated with samples that use this sample description.

Version

A 16-bit integer indicating the version number of the compressed data.

Revision level

A 16-bit integer.

Vendor

A 32-bit integer that specifies the developer of the compressor that generated the compressed data.

Temporal quality

A 32-bit integer that indicates the degree of temporal compression.

Spatial quality

A 32-bit integer that indicates the degree of spatial compression.

Width

A 16-bit integer that specifies the width of the source image in pixels.

Height

A 16-bit integer that specifies the height of the source image in pixels.

Horizontal resolution

A 32-bit fixed-point number containing the horizontal resolution of the image in pixels per inch.

Vertical resolution

A 32-bit fixed-point number containing the vertical resolution of the image in pixels per inch.

Data size

A 32-bit integer.

Frame count

A 16-bit integer that indicates how many frames of compressed data are stored in each sample.

Compressor name

A 32-byte Pascal string containing the name of the compressor that created the image, such as “jpeg”.

Depth

A 16-bit integer that indicates the pixel depth of the compressed image.

Color table ID

A 16-bit integer that identifies which color table to use.

## See Also

### Storing video data

Video sample description extensions

Extend video sample descriptions by appending other atoms.

Video sample data

Store video sample data in different formats, depending on the type of compression you use.

