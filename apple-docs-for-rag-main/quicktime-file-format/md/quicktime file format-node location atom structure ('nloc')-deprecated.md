

- QuickTime File Format
-  Node location atom structure ('nloc') Deprecated

Atom

# Node location atom structure ('nloc')

An atom that describes the type of a node and its location.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

The node location atom is the only child atom defined for the node ID atom. Its atom type is `kQTVRNodeLocationAtomType` (`'nloc'`). A node location atom describes the type of a node and its location.

The structure of a node location atom is defined by the `QTVRNodeLocationAtom` data type:

```
typedef struct VRNodeLocationAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    OSType                              nodeType;
    UInt32                              locationFlags;
    UInt32                              locationData;
    UInt32                              reserved1;
    UInt32                              reserved2;
} VRNodeLocationAtom, *QTVRNodeLocationAtomPtr;
QT
QT
```

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

nodeType

The node type.

locationFlags

The location flags.

locationData

The location of the node data.

reserved1

Reserved.

reserved2

Reserved.

## See Also

### Media data atom types

Sprite media

Sprite media is used to store character-based animation data in QuickTime movies.

Sprite track properties

Define properties that apply to an entire sprite track.

Sprite track media format

A media format for that stores sprite track information in atoms.

Sprite media atom and data types

Atoms that represent sprite media and data types.

Sprite button behaviors

Specify simple button behaviors for sprites in a sprite track.

QT atom container description key

Build QT atom container-based data structures.

Sprite media handler track properties QT atom container format

Set sprite media handler track properties in a QT atom container.

Sprite media handler sample QT atom container formats

Set sprite media handlers in QT atom containers.

Wired action grammar

Embed QT event handlers in their media samples.

Tween media

Store pairs of values to be interpolated between in QuickTime movies using tween media.

3D media

Store 3D image data in a base media in QuickTime movies.

VR media

Atoms that describe the QuickTime VR world.

Node parent atom

An atom that is the parent of one or more node ID atoms.

Custom cursor atom

An atom you use to replace the default cursors used by QuickTime VR.

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

