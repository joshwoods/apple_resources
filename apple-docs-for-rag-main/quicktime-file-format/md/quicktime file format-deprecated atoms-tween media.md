

- QuickTime File Format
- Deprecated atoms
-  Tween media 

# Tween media

Store pairs of values to be interpolated between in QuickTime movies using tween media.

## Overview

Important

Tween media is deprecated in the QuickTime file format. The information that follows documents existing content containing tween media and should not be used for new development.

Tween media is used to store pairs of values to be interpolated between in QuickTime movies. These interpolated values modify the playback of other media types by using track references and track input maps. For example, a tween media could generate gradually changing volume levels to cause a sound track to fade out. It has a media type of `'twen'`.

Every tween operation is based on a collection of one or more values from which a range of output values can be algorithmically derived. Each tween is assigned a time duration, and an output value can be generated for any time value within the duration. In the simplest kind of tween operation, a pair of values is provided as input and values between the two values are generated as output.

A tween track is a special track in a movie that is used exclusively as a modifier track. The data it contains, known as tween data, is used to generate values that modify the playback of other tracks, usually by interpolating values. The tween media handler sends these values to other media handlers; it never presents data.

## Topics

### Storing tween media

Tween sample description

An atom that contains information for converting from media time to sample number to sample location for tweens.

Tween sample data

Tween type categories

Tween QT atom container

Specify the characteristics of a tween with atoms in a tween QT atom container.

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

