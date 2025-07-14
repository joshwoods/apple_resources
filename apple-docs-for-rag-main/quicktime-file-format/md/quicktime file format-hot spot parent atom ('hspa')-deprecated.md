

- QuickTime File Format
-  Hot spot parent atom ('hspa') Deprecated

Atom

# Hot spot parent atom ('hspa')

An atom that is the parent for all hot spot atoms for the node.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

The hot spot parent atom is the parent for all hot spot atoms for the node. The atom type of the hot spot parent atom is `kQTVRHotSpotParentAtomType` (`'hspa'`) and the atom type of the each hot spot atom is `kQTVRHotSpotAtomType` (`'hots'`). The atom ID of each hot spot atom is the hot spot ID for the corresponding hot spot. The hot spot ID is determined by its color index value as it is stored in the hot spot image track.

The hot spot track is an 8-bit video track that contains color information that indicates hot spots. For more information, refer to Programming With QuickTime VR.

Each hot spot atom is the parent of a number of atoms that contain information about each hot spot.

## See Also

### Specifying node information

Node header atom ('ndhd')

An atom that describes the type and ID of a node, as well as other information about the node.

Deprecated

Hot spot information atom ('hsin')

An atom that contains general information about a hot spot.

Deprecated

Specific information atom

An atom that identified the hot spot type.

Deprecated

Link hot spot atom ('link')

An atom that specifies information for a link hot spot.

Deprecated

