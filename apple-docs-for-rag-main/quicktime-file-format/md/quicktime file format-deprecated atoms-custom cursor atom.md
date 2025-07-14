

- QuickTime File Format
- Deprecated atoms
-  Custom cursor atom 

Article

# Custom cursor atom

An atom you use to replace the default cursors used by QuickTime VR.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

The hot spot information atom, discussed in Hot spot information atom ('hsin'), allows you to indicate custom cursor IDs for particular hot spots that replace the default cursors used by QuickTime VR. QuickTime VR allows you to store your custom cursors in the VR world of the movie file.

Note

The use of resource forks for the storage of QuickTime media is deprecated in the QuickTime file format. The information that follows documents existing content and should not be used for new development. In Mac OS with a two-fork file system, custom cursors could be stored in the resource fork of the movie file. However, this implementation does not work on any other operating system platform (such as Windows).

The cursor parent atom is the parent of all of the custom cursor atoms stored in the VR world. Its atom type is `kQTVRCursorParentAtomType` (`'vrcp'`). The child atoms of the cursor parent are either cursor atoms or color cursor atoms. Their atom types are `kQTVRCursorAtomType` (`'CURS'`) and `kQTVRColorCursorAtomType` (`'crsr'`). These atoms are stored exactly as cursors or color cursors would be stored as a resource.

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

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

