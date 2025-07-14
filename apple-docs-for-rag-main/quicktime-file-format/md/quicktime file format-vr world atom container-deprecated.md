

- QuickTime File Format
-  VR world atom container Deprecated

Atom

# VR world atom container

An atom that contains name for the entire scene, the default node ID, and default imaging properties, as well as a list of the nodes contained in the QTVR track.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

The VR world atom container (VR world for short) includes such information as the name for the entire scene, the default node ID, and default imaging properties, as well as a list of the nodes contained in the QTVR track.

A VR world can also contain custom scene information. QuickTime VR ignores any atom types that it doesn’t recognize, but you can extract those atoms from the VR world using standard QuickTime atom functions.

The following shows the structure of the VR world atom container. The component atoms are defined and their structures are shown in the sections that follow.

```
VR world
├── VR world header
├── Name string
├── Imaging parent
│   ├── Panorama imaging
│   └── Panorama imaging
├── Node parent
│   ├── Node ID
│   │   └── Node location
│   ├── Node ID
│   │   └── Node location
│   ├── ...
└── Cursor parent
    ├── Cursor
    ├── Color cursor
    ├── ...
```

## See Also

### Describing VR worlds

QTVR string atom

An atom that contains a string for QuickTime VR.

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

