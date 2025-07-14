

- QuickTime File Format
-  Track name atom ('tnam') 

Atom

# Track name atom ('tnam')

An atom that provides a name for a track.

## Overview

A movie atom’s user data atom may contain a track name atom (`'tnam'`).

A track can have multiple `'tnam'` atoms with different language codes. Normally it is sufficient for each track to have a single `'tnam'` atom in the same language as the track content. Alternate tracks might also have `'tnam'` atoms; their presence implies only that the name is a good user-readable label for the track.

## Topics

### Data fields

Reserved

A 32-bit integer.

Language

A 16-bit integer holding a packed ISO 639-2/T code.

Name

A string holding the track name.

## See Also

### Atoms for user data

User data atom ('udta')

An atom where you define and store data associated with a QuickTime object.

Print to video atom ('ptv ')

An atom you use to play the movie in full-screen mode, with no window and no visible controller.

