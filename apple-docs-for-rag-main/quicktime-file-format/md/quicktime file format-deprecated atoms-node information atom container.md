

- QuickTime File Format
- Deprecated atoms
-  Node information atom container 

API Collection

# Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

The node information atom container includes general information about the node such as the node’s type, ID, and name. The node information atom container also contains the list of hot spot atoms for the node. A QuickTime VR movie contains one node information atom container for each node in the file. The routine `QTVRGetNodeInfo` allows you to obtain the node information atom container for the current node or for any other node in the movie.

The following shows the structure of the node information atom container.

```
Node information
├── Node header
├── Name string
├── Comment string
└── Hot spot parent
    ├── Hot spot
    │   ├── Hot spot information
    │   ├── Name string
    │   ├── Comment string
    │   └── Link hot spot information
    ├── Hot spot
    │   ├── Hot spot information
    │   ├── Name string
    │   ├── Comment string
    │   └── Link hot spot information
    ├── ...
```

## Topics

### Specifying node information

Node header atom ('ndhd')

An atom that describes the type and ID of a node, as well as other information about the node.

Deprecated

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

Node location atom structure ('nloc')

An atom that describes the type of a node and its location.

Deprecated

Custom cursor atom

An atom you use to replace the default cursors used by QuickTime VR.

