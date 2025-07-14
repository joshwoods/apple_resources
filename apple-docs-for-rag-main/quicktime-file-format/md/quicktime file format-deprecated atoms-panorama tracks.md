

- QuickTime File Format
- Deprecated atoms
-  Panorama tracks 

API Collection

# Panorama tracks

A track that contains information about the panoramic nodes in a scene.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

A movie’s panorama track is a track that contains information about the panoramic nodes in a scene. The media type of the panorama track is `'pano'`. Each sample in a panorama track corresponds to a single panoramic node. This sample parallels the corresponding sample in the QTVR track. Panorama tracks do not have a sample description (although QuickTime requires that you specify a placeholder sample description when you call `AddMediaSample` to add a sample to a panorama track). The sample itself contains an atom container that includes a panorama sample atom and other optional atoms.

## Topics

### Storing panorama tracks

Panorama sample atom ('pdat')

An atom that describes a single panorama.

Deprecated

Panorama image track

Store the panoramic image for a panoramic node.

Cylindrical panoramas

Store cylindrical panoramas with horizontal orientation.

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

