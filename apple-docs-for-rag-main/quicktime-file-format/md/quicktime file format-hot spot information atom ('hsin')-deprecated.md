

- QuickTime File Format
-  Hot spot information atom ('hsin') Deprecated

Atom

# Hot spot information atom ('hsin')

An atom that contains general information about a hot spot.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Mentioned in 

Custom cursor atom

## Overview

The hot spot information atom contains general information about a hot spot. Its atom type is `kQTVRHotSpotInfoAtomType` (`'hsin'`). Every hot spot atom should have a hot spot information atom as a child.

The structure of a hot spot information atom is defined by the `QTVRHotSpotInfoAtom` data type:

```
typedef struct VRHotSpotInfoAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    OSType                              hotSpotType;
    QTAtomID                            nameAtomID;
    QTAtomID                            commentAtomID;
    SInt32                              cursorID[3];
    Float32                             bestPan;
    Float32                             bestTilt;
    Float32                             bestFOV;
    FloatPoint                          bestViewCenter;
    Rect                                hotSpotRect;
    UInt32                              flags;
    UInt32                              reserved1;
    UInt32                              reserved2;
} VRHotSpotInfoAtom, *QTVRHotSpotInfoAtomPtr;
```

Note

In QuickTime VR movie files, all angular values are stored as 32-bit floating-point values that specify degrees. In addition, all floating-point values conform to the IEEE Standard 754 for binary floating-point arithmetic, in big-endian format.

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

hotSpotType

The hot spot type.

nameAtomID

The ID of the string atom that contains the name of the hot spot.

commentAtomID

The ID of the string atom that contains a comment for the hot spot.

cursorID

An array of three IDs for custom hot spot cursors.

bestPan

The best pan angle for viewing this hot spot.

bestTilt

The best tilt angle for viewing this hot spot.

bestFOV

The best field of view for viewing this hot spot.

bestViewCenter

The best view center for viewing this hot spot.

hotSpotRect

The boundary box for this hot spot, specified as the number of pixels in full panoramic space.

flags

A set of hot spot flags.

reserved1

Reserved.

reserved2

Reserved.

## See Also

### Specifying node information

Node header atom ('ndhd')

An atom that describes the type and ID of a node, as well as other information about the node.

Deprecated

Hot spot parent atom ('hspa')

An atom that is the parent for all hot spot atoms for the node.

Deprecated

Specific information atom

An atom that identified the hot spot type.

Deprecated

Link hot spot atom ('link')

An atom that specifies information for a link hot spot.

Deprecated

