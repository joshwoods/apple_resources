

- QuickTime File Format
- Panorama sample atom ('pdat')
-  reserved2 

Data field

# reserved2

Reserved.

## Overview

This field must be `0`.

Important

A new flag has been added to the flags field of the `QTVRPanoSampleAtom` data structure. This flag controls how panoramas wrap horizontally. If `kQTVRPanoFlagAlwaysWrap` is set, then the panorama wraps horizontally, regardless of the number of degrees in the panorama. If the flag is not set, then the panorama wraps only when the panorama range is 360 degrees. This is the default behavior.

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

