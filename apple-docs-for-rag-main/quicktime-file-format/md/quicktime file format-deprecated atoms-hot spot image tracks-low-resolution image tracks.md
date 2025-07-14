

- QuickTime File Format
- Deprecated atoms
- Hot spot image tracks
-  Low-resolution image tracks 

Article

# Low-resolution image tracks

Create low resolution image tracks for low memory conditions.

## Overview

It’s possible to store one or more low-resolution versions of a panoramic image in a movie file; those versions are called low-resolution image tracks. If there is not enough memory at runtime to use the normal image track, QuickTime VR uses a lower resolution image track if one is available. A low-resolution image track contains diced frames just like the higher resolution track, but the reconstructed panoramic image is half the height and half the width of the higher resolution image.

Important

The panoramic images in the lower resolution image tracks and the hot spot image tracks, if present, must have the same orientation (horizontal or vertical) as the panorama image track.

## See Also

### Hot spot image tracks

Track reference entry structure

A data structure you use to specify information about any low-resolution image tracks contained in a movie.

