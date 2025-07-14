

- QuickTime File Format
-  VR world header atom Deprecated

Atom

# VR world header atom

An atom contains the name of the scene and the default node ID to be used when the file is first opened.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

The VR world header atom is a leaf atom. Its atom type is `kQTVRWorldHeaderAtomType` (`'vrsc'`). It contains the name of the scene and the default node ID to be used when the file is first opened as well as fields reserved for future use.

The structure of a VR world header atom is defined by the `QTVRWorldHeaderAtom` data type.

```
typedef struct VRWorldHeaderAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    QTAtomID                            nameAtomID;
    UInt32                              defaultNodeID;
    UInt32                              vrWorldFlags;
    UInt32                              reserved1;
    UInt32                              reserved2;
} VRWorldHeaderAtom, *QTVRWorldHeaderAtomPtr;
QT
QT
```

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

nameAtomID

The ID of the string atom that contains the name of the scene.

defaultNodeID

The ID of the default node.

vrWorldFlags

A set of flags for the VR world.

reserved1

Reserved.

reserved2

Reserved.

## See Also

### Describing VR worlds

QTVR string atom

An atom that contains a string for QuickTime VR.

Deprecated

VR world atom container

An atom that contains name for the entire scene, the default node ID, and default imaging properties, as well as a list of the nodes contained in the QTVR track.

Deprecated

Imaging parent atom

An atom that is the parent atom of one or more node-specific imaging atoms.

Deprecated

Panorama imaging atom

An atom describes the default imaging characteristics for all the panoramic nodes in a scene.

Deprecated

