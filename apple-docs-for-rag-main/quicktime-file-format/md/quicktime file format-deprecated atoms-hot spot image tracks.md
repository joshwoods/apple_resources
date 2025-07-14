

- QuickTime File Format
- Deprecated atoms
-  Hot spot image tracks 

# Hot spot image tracks

Identify hot spots in a panorama with a hot spot image track.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

When a panorama contains hot spots, the movie file contains a hot spot image track, a video track that contains a parallel panorama, with the hot spots designated by regions filled with color. Each diced frame of the hot spot panoramic image must be compressed with a lossless compressor (such as QuickTime’s graphics compressor). The dimensions of the hot spot panoramic image are usually the same as those of the image track’s panoramic image, but this is not required. The dimensions must, however, have the same aspect ratio as the image track’s panoramic image. A hot spot image track should be 8 bits deep.

## Topics

### Hot spot image tracks

Low-resolution image tracks

Create low resolution image tracks for low memory conditions.

Track reference entry structure

A data structure you use to specify information about any low-resolution image tracks contained in a movie.

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

