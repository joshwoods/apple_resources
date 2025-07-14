

- QuickTime File Format
- Panorama sample atom ('pdat')
-  flags 

Data field

# flags

A set of panorama flags.

## Overview

`kQTVRPanoFlagHorizontal` has been superseded by the `panoType` field. It is used only when the `panoType` field is `nil` to indicate a horizontally-oriented cylindrical panorama. `kQTVRPanoFlagAlwaysWrap` is set if the panorama should wrap horizontally, regardless of whether or not the pan range is 360 degrees. Note that these flags are currently supported only under OS X.

## See Also

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

imageRefTrackIndex

The index of the image track reference.

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

