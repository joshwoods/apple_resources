

- QuickTime File Format
- Deprecated atoms
-  Panorama tracks in cubic nodes 

Article

# Panorama tracks in cubic nodes

Specify special values in the pano sample data atom to provide compatibility back to QuickTime VR 2.2.

## Overview

Important

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

The media sample for a panorama track contains the pano sample atom container. For cubes, some of the fields in the pano sample data atom have special values, which provide compatibility back to QuickTime VR 2.2. The cubic projection engine ignores these fields. They allow one to view cubic movies in older versions of QuickTime VR using the cylindrical engine, although the view will be somewhat incorrect, and the top and bottom faces will not be visible. The special values are shown in the following table.

| Field             | Value              |
|-------------------|--------------------|
| `imageNumFramesX` | `4`                |
| `imageNumFramesY` | `1`                |
| `imageSizeX`      | Frame width \* `4` |
| `imageSizeY`      | Frame height       |
| `minPan`          | `0.0`              |
| `maxPan`          | `360.0`            |
| `minTilt`         | `-45.0`            |
| `maxTilt`         | `45.0`             |
| `minFieldOfView`  | `5.0`              |
| `maxFieldOfView`  | `90.0`             |
| `flags`           | `1`                |

A `1` value in the flags field tells QuickTime VR 2.2 that the frames are not rotated. QuickTime VR 2.2 treats this as a four-frame horizontal cylinder. The `panoType` field (formerly `reserved1`) must be set to `kQTVRCube` (`'cube'`) so that QuickTime VR 3.0 can recognize this panorama as a cube.

Since certain viewing fields in the pano sample data atom are being used for backward compatibility, a new atom must be added to indicate the proper viewing parameters for the cubic image. This atom is the cubic view atom (atom type `'cuvw'`). The data structure of the cubic view atom is as follows:

```
struct QTVRCubicViewAtom {
    Float32         minPan;
    Float32         maxPan;
    Float32         minTilt;
    Float32         maxTilt;
    Float32         minFieldOfView;
    Float32         maxFieldOfView;

    Float32         defaultPan;
    Float32         defaultTilt;
    Float32         defaultFieldOfView;
};
typedef struct QTVRCubicViewAtom    QTVRCubicViewAtom;
```

The fields are filled in as desired for the cubic image. This atom is ignored by older versions of QuickTime VR. Typical minimum and maximum field values are shown in the following table.

| Field            | Value   |
|------------------|---------|
| `minPan`         | `0.0`   |
| `maxPan`         | `360.0` |
| `minTilt`        | `-90.0` |
| `maxTilt`        | `90.0`  |
| `minFieldOfView` | `5.0`   |
| `maxFieldOfView` | `120.0` |

You add the cubic view atom to the pano sample atom container (after adding the pano sample data atom). Then use `AddMediaSample` to add the atom container to the panorama track.

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

