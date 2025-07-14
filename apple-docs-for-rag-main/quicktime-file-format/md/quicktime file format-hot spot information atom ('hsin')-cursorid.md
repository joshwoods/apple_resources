

- QuickTime File Format
- Hot spot information atom ('hsin')
-  cursorID 

Data field

# cursorID

An array of three IDs for custom hot spot cursors.

## Overview

Custom hot spot cursors override the default hot spot cursors provided by QuickTime VR. The first ID (`cursorID[0]`) specifies the cursor that is displayed when it is in the hot spot. The second ID (`cursorID[1]`) specifies the cursor that is displayed when it is in the hot spot and the mouse button is down. The third ID (`cursorID[2]`) specifies the cursor that is displayed when it is in the hot spot and the mouse button is released. To retain the default cursor for any of these operations, set the corresponding cursor ID to `0`. Custom cursors should be stored in the VR world atom container, as described in VR world atom container.

## See Also

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

