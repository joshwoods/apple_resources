

- QuickTime File Format
-  QTVR string atom Deprecated

Atom

# QTVR string atom

An atom that contains a string for QuickTime VR.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

A string atom contains a string. The structure of a string atom is defined by the `QTVRStringAtom` data type.

```
typedef struct QTVRStringAtom {
    UInt16                              stringUsage;
    UInt16                              stringLength;
    unsigned char                       theString[4];
} QTVRStringAtom, *QTVRStringAtomPtr;
```

Each string atom may also have a sibling leaf atom, called the string encoding atom. The string encoding atom’s atom type is `kQTVRStringEncodingAtomType` (`'vrse'`). Its atom ID is the same as that of the corresponding string atom. The string encoding atom contains a single variable, `TextEncoding`, a `UInt32`, as defined in the header file `TextCommon.h`. The value of `TextEncoding` is handed, along with the string, to the routine `QTTextToNativeText` for conversion for display on the current machine. The routine `QTTextToNativeText` is found in the header file `Movies.h`.

Note

The header file TextCommon.h contains constants and routines for generating and handling text encodings.

## Topics

### Data fields

stringUsage

The string usage.

stringLength

The length, in bytes, of the string.

theString

The string.

## See Also

### Describing VR worlds

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

