

- QuickTime File Format
- Deprecated atoms
-  QT atom container description key 

Article

# QT atom container description key

Build QT atom container-based data structures.

## Overview

Because QT atom container–based data structures are widely used in QuickTime, a description key is presented here. Its usage is illustrated in the following sections, Sprite media handler track properties QT atom container format and Sprite media handler sample QT atom container formats.

```
[(QTAtomFormatName)] =
atomType_1, id, index
    data
atomType_n, id, index
    data
```

The atoms may be required or optional:

```
 // optional atom
 // required atom

atomType
```

The atom ID may be a number if it is required to be a constant, or it may be a list of valid atom IDs, indicating that multiple atoms of this type are allowed.

```
3               // one atom with id of 3
(1..3)          // three atoms with id's of 1, 2, and 3
(1, 5, 7)       // three atoms with id's of 1, 5, and 7
(anyUniqueIDs)  // multiple atoms each with a unique id
```

The atom index may be a `1` if only one atom of this type is allowed, or it may be a range from `1` to some constant or variable.

```
1               // one atom of this type is allowed, index is always  1
(1..3)          // three atoms with indexes 1, 2, and 3
(1..numAtoms)   // numAtoms atoms with indexes of 1 to numAtoms
```

The data may be leaf data in which its data type is listed inside of brackets \[\], or it may be a nested tree of atoms.

```
[theDataType]   // leaf data of type theDataType
childAtoms      // a nested tree of atoms
```

Nested `QTAtom` format definitions \[(AtomFormatName)\] may appear in a definition.

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

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

