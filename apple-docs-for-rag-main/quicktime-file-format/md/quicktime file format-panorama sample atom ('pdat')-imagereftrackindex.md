

- QuickTime File Format
- Panorama sample atom ('pdat')
-  imageRefTrackIndex 

Data field

# imageRefTrackIndex

The index of the image track reference.

## Overview

This is the index returned by the `AddTrackReference` function when the image track is added as a reference to the panorama track. There can be more than one image track for a given panorama track and hence multiple references. (A panorama track might have multiple image tracks if the panoramas have different characteristics, which could occur if the panoramas were shot with different size camera lenses.) The value in this field is `0` if there is no corresponding image track.

## See Also

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

hotSpotRefTrackIndex

The index of the hot spot track reference.

minPan

The minimum pan angle, in degrees.

maxPan

The maximum pan angle, in degrees.

minTilt

The minimum tilt angle, in degrees.

maxTilt

The maximum tilt angle, in degrees.

minFieldOfView

The minimum vertical field of view, in degrees.

maxFieldOfView

The maximum vertical field of view, in degrees.

defaultPan

The default pan angle, in degrees.

defaultTilt

The default tilt angle, in degrees.

defaultFieldOfView

The default vertical field of view, in degrees.

imageSizeX

The width, in pixels, of the panorama stored in the highest resolution image track.

imageSizeY

The height, in pixels, of the panorama stored in the highest resolution image track.

imageNumFramesX

The number of frames into which the panoramic image is diced horizontally.

