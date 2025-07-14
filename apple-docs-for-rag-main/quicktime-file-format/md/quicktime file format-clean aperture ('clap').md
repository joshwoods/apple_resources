

- QuickTime File Format
-  Clean aperture ('clap') 

Atom

# Clean aperture ('clap')

An extension that defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed.

## Mentioned in 

QuickTime File Format change log

## Overview

The clean aperture extension defines the relationship between the pixels in a stored image and a canonical rectangular region of a video system from which it was captured or to which it will be displayed. This can be used to correlate pixel locations in two or more images — possibly recorded using different systems — for accurate compositing. This is necessary because different video digitizer devices can digitize different regions of the incoming video signal, causing pixel misalignment between images. In particular, a stored image may contain “edge” data outside the canonical display area for a given system.

The clean aperture is either coincident with the stored image or a subset of the stored image; if it is a subset, it may be centered on the stored image, or it may be offset positively or negatively from the stored image center.

The clean aperture extension contains a width in pixels, a height in picture lines, and a horizontal and vertical offset between the stored image center and a canonical image center for the given video system. The width is typically the width of the canonical clean aperture for a video system divided by the pixel aspect ratio of the stored data. The offsets also take into account any “overscan” in the stored image. The height and width must be positive values, but the offsets may be positive, negative, or zero.

These values are given as ratios of two 32-bit numbers, so that applications can calculate precise values with minimum roundoff error. For whole values, the value should be stored in the numerator field while the denominator field is set to `1`.

## Topics

### Data fields

Size

A 32-bit unsigned integer.

Type

A 32-bit unsigned integer.

apertureWidth_N

A 32-bit signed integer containing either the width of the clean aperture in pixels or the numerator portion of a fractional width.

apertureWidth_D

A 32-bit signed integer containing either the denominator portion of a fractional width or the number 1.

apertureHeight_N

A 32-bit signed integer containing either the height of the clean aperture in picture lines or the numerator portion of a fractional height.

apertureHeight_D

A 32-bit signed integer containing either the denominator portion of a fractional height or the number 1.

horizOff_N

A 32-bit signed integer containing either the horizontal offset of the clean aperture center minus (width–1)/2 or the numerator portion of a fractional offset.

horizOff_D

A 32-bit signed integer containing either the denominator portion of the horizontal offset or the number 1.

vertOff_N

A 32-bit signed integer containing either the vertical offset of the clean aperture center minus (height–1)/2 or the numerator portion of a fractional offset.

vertOff_D

A 32-bit signed integer containing either the denominator portion of the vertical offset or the number 1.

## See Also

### Extending video sample descriptions

Pixel aspect ratio ('pasp')

An extension that specifies the height-to-width ratio of pixels found in the video sample.

MPEG-4 elementary stream descriptor atom ('esds')

A required extension to the video sample description for MPEG-4 video.

AVC decoder configuration atom ('avcC')

A required extension to the video sample description for H.264 video.

Color parameter atom ('colr')

A required extension for uncompressed Y´CbCr data formats.

