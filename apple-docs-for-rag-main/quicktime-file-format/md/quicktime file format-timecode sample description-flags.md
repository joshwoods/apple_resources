

- QuickTime File Format
- Timecode sample description
-  Flags 

Data field

# Flags

A 32-bit integer containing flags that identify some timecode characteristics.

## Overview

The following flags are defined:

Drop frame  
Indicates whether the timecode is drop frame. Set it to `1` if the timecode is drop frame. This flag’s value is `0x0001`.

24 hour max  
Indicates whether the timecode wraps after 24 hours. Set it to `1` if the timecode wraps. This flag’s value is `0x0002`.

Negative times OK  
Indicates whether negative time values are allowed. Set it to `1` if the timecode supports negative values. This flag’s value is `0x0004`.

Counter  
Indicates whether the time value corresponds to a tape counter value. Set it to `1` if the timecode values are tape counter values. This flag’s value is `0x0008`.

## See Also

### Data fields

Reserved

A 32-bit integer that is reserved for future use.

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

