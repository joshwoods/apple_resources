

- QuickTime File Format
-  kTweenRegionData Deprecated

Atom

# kTweenRegionData

An atom that contains the data for a QuickDraw region.

Deprecated

Tween media is deprecated in the QuickTime file format. The information that follows documents existing content containing tween media and should not be used for new development.

## Overview

Used only by a `kTweenTypeQDRegion` atom.

Its parent atom is a `kTweenEntry` atom.

A `kTweenEntry` atom can contain only one `kTweenRegionData` or `kTweenPictureData` atom. The ID of this atom is always `1`. The index of this atom is always `1`.

This atom is a leaf atom. The data type of its data is `Region`.

Either a `kTweenPictureData` or `kTweenRegionData` atom is required for a `kTweenTypeQDRegion` tween.

## See Also

### Region Tween Atoms

kTweenPictureData

An atom that contains the data for a QuickDraw picture.

Deprecated

kTweenSequenceElement

An atom that specifies an entry in a tween sequence.

Deprecated

