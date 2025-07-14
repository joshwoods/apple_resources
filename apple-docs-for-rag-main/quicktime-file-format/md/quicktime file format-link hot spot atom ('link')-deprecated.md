

- QuickTime File Format
-  Link hot spot atom ('link') Deprecated

Atom

# Link hot spot atom ('link')

An atom that specifies information for a link hot spot.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

The link hot spot atom specifies information for hot spots of type `kQTVRHotSpotLinkType` (’`link'`). Its atom type is thus `'link'`. The link hot spot atom contains specific information about a link hot spot.

The structure of a link hot spot atom is defined by the `QTVRLinkHotSpotAtom` data type:

```
typedef struct VRLinkHotSpotAtom {
    UInt16                              majorVersion;
    UInt16                              minorVersion;
    UInt32                              toNodeID;
    UInt32                              fromValidFlags;
    Float32                             fromPan;
    Float32                             fromTilt;
    Float32                             fromFOV;
    FloatPoint                          fromViewCenter;
    UInt32                              toValidFlags;
    Float32                             toPan;
    Float32                             toTilt;
    Float32                             toFOV;
    FloatPoint                          toViewCenter;
    Float32                             distance;
    UInt32                              flags;
    UInt32                              reserved1;
    UInt32                              reserved2;
} VRLinkHotSpotAtom, *VRLinkHotSpotAtomPtr;
```

Certain fields in the link hot spot atom are not used by QuickTime VR. The `fromValidFlags` field is generally set to 0 and the other `from` fields are not used. However, these fields could be quite useful if you have created a transition movie from one node to another. The from angles can be used to swing the current view of the source node to align with the first frame of the transition movie. The `distance` field is intended for use with 3D applications, but is also not used by QuickTime VR.

## Topics

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

toNodeID

The ID of the destination node.

fromValidFlags

A set of flags that indicate which source node view settings are valid.

fromPan

The preferred from-pan angle at the source node.

fromTilt

The preferred from-tilt angle at the source node.

fromFOV

The preferred from-field of view at the source node.

fromViewCenter

The preferred from-view center at the source node.

toValidFlags

A set of flags that indicate which destination node view settings are valid.

toPan

The pan angle to use when displaying the destination node.

toTilt

The tilt angle to use when displaying the destination node.

toFOV

The field of view to use when displaying the destination node.

toViewCenter

The view center to use when displaying the destination node.

distance

The distance between the source node and the destination node.

flags

A set of link hot spot flags.

reserved1

Reserved.

reserved2

Reserved.

## See Also

### Specifying node information

Node header atom ('ndhd')

An atom that describes the type and ID of a node, as well as other information about the node.

Deprecated

Hot spot parent atom ('hspa')

An atom that is the parent for all hot spot atoms for the node.

Deprecated

Hot spot information atom ('hsin')

An atom that contains general information about a hot spot.

Deprecated

Specific information atom

An atom that identified the hot spot type.

Deprecated

