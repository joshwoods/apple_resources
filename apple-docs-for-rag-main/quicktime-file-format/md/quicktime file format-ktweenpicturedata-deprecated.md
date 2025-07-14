

- QuickTime File Format
-  kTweenPictureData Deprecated

Atom

# kTweenPictureData

An atom that contains the data for a QuickDraw picture.

Deprecated

Tween media is deprecated in the QuickTime file format. The information that follows documents existing content containing tween media and should not be used for new development.

## Overview

Used only by a `kTweenTypeQDRegion` atom.

Its parent atom is a `kTweenEntry` atom.

A `kTweenEntry` atom can contain only one `kTweenPictureData` or `kTweenRegionData` atom. The ID of this atom is always `1`. The index of this atom is always `1`.

This atom is a leaf atom. The data type of its data is `Picture`.

Either a `kTweenPictureData` or `kTweenRegionData` atom is required for a `kTweenTypeQDRegion` atom.

## See Also

### Region Tween Atoms

kTweenRegionData

An atom that contains the data for a QuickDraw region.

Deprecated

kTweenSequenceElement

An atom that specifies an entry in a tween sequence.

Deprecated

