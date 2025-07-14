

- QuickTime File Format
-  Timecode sample description 

Atom

# Timecode sample description

An atom that defines how to interpret time code media data.

## Overview

The timecode sample description contains information that defines how to interpret time code media data. This sample description is based on the standard sample description header, as described in Sample description atom ('stsd').

The data format field in the sample description is always set to `'tmcd'`.

The timecode media handler also adds some of its own fields to the sample description.

## Topics

### Data fields

Reserved

A 32-bit integer that is reserved for future use.

Flags

A 32-bit integer containing flags that identify some timecode characteristics.

Time scale

A 32-bit integer that specifies the time scale for interpreting the frame duration field.

Frame duration

A 32-bit integer that indicates how long each frame lasts in real time.

Number of frames

An 8-bit integer that contains the number of frames per second for the timecode format.

Reserved

An 8-bit quantity.

Source reference

A user data atom containing information about the source tape.

## See Also

### Storing time code data

Timecode media information atom ('tcmi')

An atom that governs how the timecode text is displayed.

Timecode sample data

An atom that represents timecode sample data.

Creating a timecode track for 29.97 FPS video

Configure a timecode track to specify timecode information for other tracks.

