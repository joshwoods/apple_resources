

- QuickTime File Format
- Deprecated atoms
-  3D media 

Article

# 3D media

Store 3D image data in a base media in QuickTime movies.

## Overview

Important

3D Media is deprecated in the QuickTime file format. The information that follows documents existing content containing 3D media and should not be used for new development.

QuickTime movies store 3D image data in a base media. This media has a media type of `'qd3d'`.

## 3D Sample Description

The 3D sample description uses the standard sample description header, as described in Sample table atom ('stbl').

The data format field in the sample description is always set to `'qd3d'`. The 3D media handler adds no additional fields to the sample description.

## 3D Sample Data

The 3D samples are stored in the 3D Metafile format developed for QuickDraw 3D.

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

