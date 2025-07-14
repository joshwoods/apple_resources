

- QuickTime File Format
-  Hint sample data format 

Atom

# Hint sample data format

An atom that specifies the data format and location of the hint track sample data.

## Overview

The sample description atom (`'stsd'`) contains information about the hint track samples. It specifies the data format (note that currently only RTP data format is defined) and the data reference to use (if more than one is defined) to locate the hint track sample data. It also contains some general information about this hint track, such as the hint track version number, the maximum packet size allowed by this hint track, and the RTP time scale. It may contain additional information, such as the random offsets to add to the RTP time stamp and sequence number.

The sample description atom can contain a table of sample descriptions to accommodate media that are encoded in multiple formats, but a hint track can be expected to have a single sample description at this time.

The sample description for hint tracks is defined in the following table.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Data format | 4 |
| Reserved | 6 |
| Data reference index | 2 |
| Hint track version | 2 |
| Last compatible hint track version | 2 |
| Max packet size | 4 |
| Additional data table | variable |

## Topics

### Data fields

Size

A 32-bit integer specifying the size of this sample description in bytes.

Data format

A four-character code indicating the data format of the hint track samples.

Reserved

Six bytes.

Data reference index

A field that indirectly specifies where to find the hint track sample data.

Hint track version

A 16-bit unsigned integer indicating the version of the hint track specification.

Last compatible hint track version

A 16-bit unsigned integer indicating the oldest hint track version with which this hint track is backward-compatible.

Max packet size

A 32-bit integer indicating the packet size limit, in bytes, used when creating this hint track.

Additional data table

A table of variable length containing additional information.

## See Also

### Hint media

Hint media

Provide information about data units to stream in hint tracks.

Finding an original media track from a hint track

Use track reference atoms from hint tracks to locate the original media track.

RTP hint tracks

Allow a streaming server to create RTP streams from a QuickTime movie.

Packetization hint sample data

An atom that describes the sample data for data using the Real-Time Transport Protocol (RTP).

