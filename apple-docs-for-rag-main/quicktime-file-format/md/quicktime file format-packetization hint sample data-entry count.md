

- QuickTime File Format
- Packetization hint sample data
-  Entry count 

Data field

# Entry count

A 16-bit unsigned integer indicating the number of packet entries in the table.

## Overview

Each entry in the table corresponds to a packet. Multiple entries in a single sample indicate that the media sample had to be split into multiple packets. A sample with an entry count of `0` is reserved and, if encountered, must be skipped.

## See Also

### Data fields

Reserved

Two bytes.

Packet entry table

A variable length table containing packet entries.

Additional data

A variable length field containing data pointed to by the entries in the data table.

