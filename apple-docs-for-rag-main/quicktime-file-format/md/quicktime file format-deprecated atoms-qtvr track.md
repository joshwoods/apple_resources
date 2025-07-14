

- QuickTime File Format
- Deprecated atoms
-  QTVR track 

API Collection

# QTVR track

A track that maintains a list of all the nodes in a movie.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

A QTVR track is a special type of QuickTime track that maintains a list of all the nodes in a movie. The media type for a QTVR track is `'qtvr'`. All the media samples in a QTVR track share a common sample description. This sample description contains the VR world atom container. The track contains one media sample for each node in the movie. Each QuickTime VR media sample contains a node information atom container.

## Topics

### Storing sample descriptions

QuickTime VR sample description ('qtvr')

Describe QuickTime VR samples.

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

