

- QuickTime File Format
- Deprecated atoms
-  Object tracks 

API Collection

# Object tracks

A track that contains information about the object nodes in a scene.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

A movie’s object track is a track that contains information about the object nodes in a scene. The media type of the object track is `'obje'`. Each sample in an object track corresponds to a single object node in the scene. The samples of the object track contain information describing the object images stored in the object image track.

These object information samples parallel the corresponding node samples in the QTVR track and are equal in time and duration to a particular object node’s image samples in the object’s image track as well as the object node’s hot spot samples in the object’s hot spot track.

Object tracks do not have a sample description (although QuickTime requires that you specify a placeholder sample description when you call `AddMediaSample` to add a sample to an object track). The sample itself is an atom container that contains a single object sample atom and other optional atoms.

## Topics

### Storing object tracks

Object sample atom

An atom that describes a single object.

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

