

- QuickTime File Format
- Deprecated atoms
-  Sprite track properties 

Article

# Sprite track properties

Define properties that apply to an entire sprite track.

## Overview

Important

Sprite media is deprecated in the QuickTime file format. The information that follows documents existing content containing sprite media and should not be used for new development.

In addition to defining properties for individual sprites, you can also define properties that apply to an entire sprite track. These properties may override default behavior or provide hints to the sprite media handler. The following sprite track properties are supported:

`kSpriteTrackPropertyBackgroundColor`  
Specifies a background color for the sprite track. The background color is used for any area that is not covered by regular sprites or background sprites. If you do not specify a background color, the sprite track uses black as the default background color.

`kSpriteTrackPropertyOffscreenBitDepth`  
Specifies a preferred bit depth for the sprite track’s offscreen buffer. The allowable values are 8 and 16. To save memory, you should set the value of this property to the minimum depth needed. If you do not specify a bit depth, the sprite track allocates an offscreen buffer with the depth of the deepest intersecting monitor.

`kSpriteTrackPropertySampleFormat`  
Specifies the sample format for the sprite track. If you do not specify a sample format, the sprite track uses the default format, `kKeyFrameAndSingleOverride`.

To specify sprite track properties, you create a single QT atom container and add a leaf atom for each property you want to specify. To add the properties to a sprite track, you call the media handler function `SetMediaPropertyAtom`. To retrieve a sprite track’s properties, you call the media handler function `GetMediaPropertyAtom`.

The sprite track properties and their corresponding data types are listed in the following table.

| Atom type                                      | Atom ID | Leaf data type   |
|------------------------------------------------|---------|------------------|
| `kSpriteTrackPropertyBackgroundColor`          | `1`     | `RGBColor`       |
| `kSpriteTrackPropertyOffscreenBitDepth`        | `1`     | `unsigned short` |
| `kSpriteTrackPropertySampleFormat`             | `1`     | `long`           |
| `kSpriteTrackPropertyHasActions`               | `1`     | `Boolean`        |
| `kSpriteTrackPropertyQTIdleEventsFrequency`    | `1`     | `UInt32`         |
| `kSpriteTrackPropertyVisible`                  | `1`     | `Boolean`        |
| `kSpriteTrackPropertyScaleSpritesToScaleWorld` | `1`     | `Boolean`        |

Note

When pasting portions of two different tracks together, the Movie Toolbox checks to see that all sprite track properties match. If, in fact, they do match, the paste results in a single sprite track instead of two.

## See Also

### Media data atom types

Sprite media

Sprite media is used to store character-based animation data in QuickTime movies.

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

Node information atom container

An atom container that includes general information about the node such as the node’s type, ID, and name.

