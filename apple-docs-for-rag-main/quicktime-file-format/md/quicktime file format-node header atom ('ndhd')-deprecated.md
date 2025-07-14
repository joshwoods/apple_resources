

- QuickTime File Format
-  Node header atom ('ndhd') Deprecated

Atom

# Node header atom ('ndhd')

An atom that describes the type and ID of a node, as well as other information about the node.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

A node header atom is a leaf atom that describes the type and ID of a node, as well as other information about the node. Its atom type is `kQTVRNodeHeaderAtomType` (`'ndhd'`).

The structure of a node header atom is defined by the QTVRNodeHeaderAtom data type:

```
typedef struct VRNodeHeaderAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    OSType                              nodeType;
    QTAtomID                            nodeID;
    QTAtomID                            nameAtomID;
    QTAtomID                            commentAtomID;
    UInt32                              reserved1;
    UInt32                              reserved2;
} VRNodeHeaderAtom, *VRNodeHeaderAtomPtr;
```

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

nodeType

The node type.

nodeID

The node ID.

nameAtomID

The ID of the string atom that contains the name of the node.

commentAtomID

The ID of the string atom that contains a comment for the node.

reserved1

Reserved.

reserved2

Reserved.

## See Also

### Specifying node information

Hot spot parent atom ('hspa')

An atom that is the parent for all hot spot atoms for the node.

Deprecated

Hot spot information atom ('hsin')

An atom that contains general information about a hot spot.

Deprecated

Specific information atom

An atom that identified the hot spot type.

Deprecated

Link hot spot atom ('link')

An atom that specifies information for a link hot spot.

Deprecated

