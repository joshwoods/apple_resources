

- QuickTime File Format
- Packet entry
-  Flags 

Data field

# Flags

A 16-bit field indicating certain attributes for this packet.

## Overview

Defined bits are shown in the following table.

| Bit  | Value    |
|------|----------|
| 0-12 | reserved |
| 3    | X        |
| 4    | B        |
| 5    | R        |

## See Also

### Data fields

Relative packet transmission time

A 32-bit signed integer value, indicating the time, in the hint track’s time scale, to send this packet relative to the hint sample’s actual time.

RTP header info

A 16-bit integer specifying various values to be set in the RTP header.

RTP sequence number

A 16-bit integer specifying the RTP sequence number for this packet.

Entry count

A 16-bit unsigned integer specifying the number of entries in the data table.

Extra information TLVs

A list of extra informtion that extends the hint track format without changing the version.

Data table

A table that defines the data to be put in the payload portion of the RTP packet.

