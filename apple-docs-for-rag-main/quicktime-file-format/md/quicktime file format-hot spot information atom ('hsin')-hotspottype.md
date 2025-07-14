

- QuickTime File Format
- Hot spot information atom ('hsin')
-  hotSpotType 

Data field

# hotSpotType

The hot spot type.

## Overview

This type specifies which other information atoms — if any — are siblings to this one. QuickTime VR recognizes three types: `kQTVRHotSpotLinkType`, `kQTVRHotSpotURLType`, and `kQTVRHotSpotUndefinedType`.

## See Also

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

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

