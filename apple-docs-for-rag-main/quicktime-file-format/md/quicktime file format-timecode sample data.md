

- QuickTime File Format
-  Timecode sample data 

Atom

# Timecode sample data

An atom that represents timecode sample data.

## Overview

A timecode media sample is recorded as a 32-bit integer, interpreted based on the value of the Counter flag in the timecode sample description.

If the Counter flag is set to `1` in the timecode sample description, the sample data is an unsigned 32-bit integer. The timecode counter value is determined by dividing this unsigned 32-bit integer by the number of frames field in the timecode sample description.

If the Counter flag is set to `0` in the timecode sample description, the sample data format is a signed 32-bit integer and is used to calculate a timecode record.

## Topics

### Data fields

Hours

An 8-bit unsigned integer that indicates the starting number of hours.

Negative

A 1-bit value indicating the time’s sign.

Minutes

A 7-bit integer that contains the starting number of minutes.

Seconds

An 8-bit unsigned integer indicating the starting number of seconds.

Frames

An 8-bit unsigned integer that specifies the starting number of frames.

## See Also

### Storing time code data

Timecode sample description

An atom that defines how to interpret time code media data.

Timecode media information atom ('tcmi')

An atom that governs how the timecode text is displayed.

Creating a timecode track for 29.97 FPS video

Configure a timecode track to specify timecode information for other tracks.

