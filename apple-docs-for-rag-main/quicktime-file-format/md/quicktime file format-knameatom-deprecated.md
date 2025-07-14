

- QuickTime File Format
-  kNameAtom Deprecated

Atom

# kNameAtom

An atom that specifies the name of a tween atom.

Deprecated

Tween media is deprecated in the QuickTime file format. The information that follows documents existing content containing tween media and should not be used for new development.

## Overview

The name, which is optional, is not used by tween components, but it can be used by applications or other software.

Its parent atom is a `kTweenEntry` atom.

A `kTweenEntry` atom can contain only one `kNameAtom` atom. The ID of this atom is always `1`. The index of this atom is always `1`.

This atom is a leaf atom. Its data type is `String`.

This atom is optional. If it is not included, the tween atom does not have a name.

## See Also

### General tween atoms

kTweenEntry

A tween atom, which can be either a single tween atom, a tween atom in a tween sequence, or an interpolation tween atom.

Deprecated

kTweenStartOffset

An atom that specifies a time offset from the start of the tween media sample to the start of the tween atom.

Deprecated

kTweenDuration

An atom that specifies the duration of a tween operation.

Deprecated

kTweenData

An atom that contains data for a tween atom.

Deprecated

kTweenType

An atom that specifies the tween type, which is the data type of the data for the tween operation.

Deprecated

