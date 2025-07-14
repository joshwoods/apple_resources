

- QuickTime File Format
-  Object sample atom Deprecated

Atom

# Object sample atom

An atom that describes a single object.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

An object sample atom describes a single object, including information about the default viewing angles and the view settings. The structure of an object sample atom is defined by the `QTVRObjectSampleAtom` data type:

```
typedef struct VRObjectSampleAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    UInt16                              movieType;
    UInt16                              viewStateCount;
    UInt16                              defaultViewState;
    UInt16                              mouseDownViewState;
    UInt32                              viewDuration;
    UInt32                              columns;
    UInt32                              rows;
    Float32                             mouseMotionScale;
    Float32                             minPan;
    Float32                             maxPan;
    Float32                             defaultPan;
    Float32                             minTilt;
    Float32                             maxTilt;
    Float32                             defaultTilt;
    Float32                             minFieldOfView;
    Float32                             fieldOfView;
    Float32                             defaultFieldOfView;
    Float32                             defaultViewCenterH;
    Float32                             defaultViewCenterV;
    Float32                             viewRate;
    Float32                             frameRate;
    UInt32                              animationSettings;
    UInt32                              controlSettings;
} VRObjectSampleAtom, *VRObjectSampleAtomPtr;
QT
QT
QT
```

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

movieType

The movie controller type.

viewStateCount

The number of view states of the object.

defaultViewState

The 1-based index of the default view state.

mouseDownViewState

The 1-based index of the mouse-down view state.

viewDuration

The total movie duration of all image frames contained in an object’s view.

columns

The number of columns in the object image array.

rows

The number of rows in the object image array.

mouseMotionScale

The mouse motion scale factor.

minPan

The minimum pan angle, in degrees.

maxPan

The maximum pan angle, in degrees.

defaultPan

The default pan angle, in degrees.

minTilt

The minimum tilt angle, in degrees.

maxTilt

The maximum tilt angle, in degrees.

defaultTilt

The default tilt angle, in degrees.

minFieldOfView

The minimum field of view to which the object can zoom.

fieldOfView

The image field of view, in degrees, for the entire object.

defaultFieldOfView

The default field of view for the object.

defaultViewCenterH

The default horizontal view center.

defaultViewCenterV

The default vertical view center.

viewRate

The view rate.

frameRate

The frame rate.

animationSettings

A set of 32-bit flags that encode information about the animation settings of the object.

controlSettings

A set of 32-bit flags that encode information about the control settings of the object.

