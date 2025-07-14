

- QuickTime File Format
- Deprecated atoms
-  VR media 

API Collection

# VR media

Atoms that describe the QuickTime VR world.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

This section describes the QuickTime VR world and node information atom containers, which can be obtained by calling the QuickTime VR Manager routines `QTVRGetVRWorld` and `QTVRGetNodeInfo`. Those routines, as well as a complete discussion of QuickTime VR and how your application can create QuickTime VR movies, are described in detail in QuickTime VR.

Many atom types contained in the VR world and node information atom containers are unique within their container. For example, each has a single header atom. Most parent atoms within an atom container are unique as well, such as the node parent atom in the VR world atom container or the hot spot parent atom in the node information atom container. For these one-time-only atoms, the atom ID is always set to `1`. Unless otherwise mentioned in the descriptions of the atoms that follow, assume that the atom ID is `1`.

Note that many atom structures contain two version fields, `majorVersion` and `minorVersion`. The values of these fields correspond to the constants `kQTVRMajorVersion` and `kQTVRMinorVersion` found in the header file `QuickTimeVRFormat.h`. For QuickTime 2.0 files, these values are `2` and `0`.

QuickTime provides a number of routines for both creating and accessing atom containers.

Some of the leaf atoms within the VR world and node information atom containers contain fields that specify the ID of string atoms that are siblings of the leaf atom. For example, the VR world header atom contains a field for the name of the scene. The string atom is a leaf atom whose atom type is `kQTVRStringAtomType` (`'vrsg'`). Its atom ID is that specified by the referring leaf atom.

## Topics

### Describing VR worlds

QTVR string atom

An atom that contains a string for QuickTime VR.

Deprecated

VR world atom container

An atom that contains name for the entire scene, the default node ID, and default imaging properties, as well as a list of the nodes contained in the QTVR track.

Deprecated

VR world header atom

An atom contains the name of the scene and the default node ID to be used when the file is first opened.

Deprecated

Imaging parent atom

An atom that is the parent atom of one or more node-specific imaging atoms.

Deprecated

Panorama imaging atom

An atom describes the default imaging characteristics for all the panoramic nodes in a scene.

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

Node parent atom

An atom that is the parent of one or more node ID atoms.

Node location atom structure ('nloc')

An atom that describes the type of a node and its location.

Deprecated

Custom cursor atom

An atom you use to replace the default cursors used by QuickTime VR.

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

