

- QuickTime File Format
- Packet entry
-  Data table 

Data field

# Data table

A table that defines the data to be put in the payload portion of the RTP packet.

## Mentioned in 

Data modes

## Overall

This table defines various places the data can be retrieved. Table entries are listed in the following table.

| Data table entry | Bytes |
|------------------|-------|
| Data source      | 1     |
| Data             | 15    |

The data source field of the entry table indicates how the other 15 bytes of the entry are to be interpreted. Values of `0` through `4` are defined. The various data table formats are defined in Data modes.

Although there are various schemes, note that the entries in the various schemes are the same size, 16 bytes long.

## See Also

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

