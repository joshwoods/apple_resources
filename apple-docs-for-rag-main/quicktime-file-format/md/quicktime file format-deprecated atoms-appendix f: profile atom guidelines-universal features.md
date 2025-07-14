

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
-  Universal features 

# Universal features

Features that you include in any file that includes a profile atom.

## Overview

A feature consists of four fields: a reserved field, which is set to zero; a part-ID, which specifies which brand the feature belongs to; a feature code, which identifies the feature; and a value field, which holds the feature value).

The part-ID can be either universal or brand-specific. Universal features have a part-ID of four ASCII spaces (`0x20202020`). Brand-specific features have a part-ID for a particular brand, which is taken from the Compatible_brands field of the file type atom. Brand-specific features of QuickTime files have a part-ID of `'qt '`. All features listed in this section are universal features; that is, they can be used in any file that includes a profile atom.

It is permissible to use the feature code of `0x00000000` as a placeholder, paired with a feature value of `0x00000000` for one or more features. Readers should simply ignore features having a feature code of zero.

No feature will exist to describe the unit of other features, such as bit rate. The device should consider the magnitude and tailor its display appropriately.

This specification describes only how features are stored in files. It does not require that the values of features be reported (for example, in a user interface) in the same manner as they are stored, or require that they be reported at all.

## Topics

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime video codec type

QuickTime audio codec type

MPEG-4 video profile

MPEG-4 video codec

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

Audio sample rate for a sample entry

Audio variable bit rate indication

Audio channel count

## See Also

### Building a profile atom

About this appendix

Profile atom ('prfl')

An atom that expresses profiles or feature codes for features that occur in the movie.

Deprecated

