

- QuickTime File Format
-  Packet entry 

Atom

# Packet entry

A packet entry.

## Overview

The packet entry contains the data elements listed in the following table.

| Packet entry | Bytes |
|----|----|
| Relative packet transmission time | 4 |
| RTP header info | 2 |
| RTP sequence number | 2 |
| Flags | 2 |
| Entry count | 2 |
| Extra information TLVs | 0 or variable |
| Data table | variable |

## Topics

### Data fields

Relative packet transmission time

A 32-bit signed integer value, indicating the time, in the hint track’s time scale, to send this packet relative to the hint sample’s actual time.

RTP header info

A 16-bit integer specifying various values to be set in the RTP header.

RTP sequence number

A 16-bit integer specifying the RTP sequence number for this packet.

Flags

A 16-bit field indicating certain attributes for this packet.

Entry count

A 16-bit unsigned integer specifying the number of entries in the data table.

Extra information TLVs

A list of extra informtion that extends the hint track format without changing the version.

Data table

A table that defines the data to be put in the payload portion of the RTP packet.

