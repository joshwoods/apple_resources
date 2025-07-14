

- QuickTime File Format
-  Panorama sample atom ('pdat') Deprecated

Atom

# Panorama sample atom ('pdat')

An atom that describes a single panorama.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

A panorama sample atom has an atom type of `kQTVRPanoSampleDataAtomType` (`'pdat'`). It describes a single panorama, including track reference indexes of the scene and hot spot tracks and information about the default viewing angles and the source panoramic image.

The structure of a panorama sample atom is defined by the `QTVRPanoSampleAtom` data type:

```
typedef struct VRPanoSampleAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    UInt32                              imageRefTrackIndex;
    UInt32                              hotSpotRefTrackIndex;
    Float32                             minPan;
    Float32                             maxPan;
    Float32                             minTilt;
    Float32                             maxTilt;
    Float32                             minFieldOfView;
    Float32                             maxFieldOfView;
    Float32                             defaultPan;
    Float32                             defaultTilt;
    Float32                             defaultFieldOfView;
    UInt32                              imageSizeX;
    UInt32                              imageSizeY;
    UInt16                              imageNumFramesX;
    UInt16                              imageNumFramesY;
    UInt32                              hotSpotSizeX;
    UInt32                              hotSpotSizeY;
    UInt16                              hotSpotNumFramesX;
    UInt16                              hotSpotNumFramesY;
    UInt32                              flags;
    OSType                              panoType;
    UInt32                              reserved2;
} VRPanoSampleAtom, *VRPanoSampleAtomPtr;
```

The minimum and maximum values in the panorama sample atom describe the physical limits of the panoramic image. QuickTime VR allows you to set further constraints on what portion of the image a user can see by calling the `QTVRSetConstraints` routine. You can also preset image constraints by adding constraint atoms to the panorama sample atom container. The three constraint atom types are `kQTVRPanConstraintAtomType`, `kQTVRTiltConstraintAtomType`, and `kQTVRFOVConstraintAtomType`. Each of these atom types share a common structure defined by the `QTVRAngleRangeAtom` data type:

```
typedef struct QTVRAngleRangeAtom {
    Float32                             minimumAngle;
    Float32                             maximumAngle;
} QTVRAngleRangeAtom, *QTVRAngleRangeAtomPtr;
```

**Field descriptions**

`minimumAngle`  
The minimum angle in the range, in degrees.

`maximumAngle`  
The maximum angle in the range, in degrees.

## Topics

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

imageNumFramesX

The number of frames into which the panoramic image is diced horizontally.

imageNumFramesY

The number of frames into which the panoramic image is diced vertically.

hotSpotSizeX

The width, in pixels, of the panorama stored in the highest resolution hot spot image track.

hotSpotSizeY

The height, in pixels, of the panorama stored in the highest resolution hot spot image track.

hotSpotNumFramesX

The number of frames into which the panoramic image is diced horizontally for the hot spot image track.

hotSpotNumFramesY

The number of frames into which the panoramic image is diced vertically for the hot spot image track.

flags

A set of panorama flags.

panoType

An OSType describing the type of panorama.

reserved2

Reserved.

## See Also

### Storing panorama tracks

Panorama image track

Store the panoramic image for a panoramic node.

Cylindrical panoramas

Store cylindrical panoramas with horizontal orientation.

