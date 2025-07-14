

- QuickTime File Format
-  Timecode media information atom ('tcmi') 

Atom

# Timecode media information atom ('tcmi')

An atom that governs how the timecode text is displayed.

## Mentioned in 

QuickTime File Format change log

## Overview

The timecode media also requires a media information atom. This atom contains information governing how the timecode text is displayed. This media information atom is stored in a base media information atom (see Base media information atom ('minf') for more information). The type of the timecode media information atom is `'tcmi'`.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this time code media information atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this timecode media information atom.

Flags

A 3-byte space for timecode media information flags.

Text font

A 16-bit integer that indicates the font to use.

Text face

A 16-bit integer that indicates the font’s style.

Text size

A 16-bit integer that specifies the point size of the time code text.

Reserved

A 16-bit integer that is reserved for use by Apple.

Text color

A 48-bit RGB color value for the timecode text.

Background color

A 48-bit RGB background color for the timecode text.

Font name

A Pascal string specifying the name of the timecode text’s font.

## See Also

### Storing time code data

Timecode sample description

An atom that defines how to interpret time code media data.

Timecode sample data

An atom that represents timecode sample data.

Creating a timecode track for 29.97 FPS video

Configure a timecode track to specify timecode information for other tracks.

