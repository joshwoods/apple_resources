

- QuickTime File Format
- Packet entry
-  RTP sequence number 

Data field

# RTP sequence number

A 16-bit integer specifying the RTP sequence number for this packet.

## Overview

The RTP server adds a random offset to this sequence number before transmitting the packet. This field allows re-transmission of packets—for example, the same packet can be assembled with the same sequence number and a different (later) packet transmission time. A text sample with a duration of 5 minutes can be retransmitted every 10 seconds, so that clients that miss the original sample transmission (perhaps they started playing the movie in the middle) will be refreshed after a maximum of 10 seconds.

## See Also

### Data fields

Relative packet transmission time

A 32-bit signed integer value, indicating the time, in the hint track’s time scale, to send this packet relative to the hint sample’s actual time.

RTP header info

A 16-bit integer specifying various values to be set in the RTP header.

Flags

A 16-bit field indicating certain attributes for this packet.

Entry count

A 16-bit unsigned integer specifying the number of entries in the data table.

Extra information TLVs

A list of extra informtion that extends the hint track format without changing the version.

Data table

A table that defines the data to be put in the payload portion of the RTP packet.

