

- QuickTime File Format
-  Packetization hint sample data 

Atom

# Packetization hint sample data

An atom that describes the sample data for data using the Real-Time Transport Protocol (RTP).

## Overview

This section describes the sample data for the `'rtp '` format. The `'rtp '` format assumes that the server is sending data using Real-Time Transport Protocol (RTP). This format also assumes that the server “knows” about RTP headers but does not require that the server know anything about specific media headers, including media headers defined in various IETF drafts.

Each sample in the hint track will generate one or more RTP packets. Each entry in the sample data table in a hint track sample corresponds to a single RTP packet. Samples in the hint track may or may not correspond exactly to samples in the media track. Data in the hint track sample is byte aligned, but not 32-bit aligned.

The RTP timestamps of all packets in a hint sample are the same as the hint sample time. In other words, packets that do not have the same RTP timestamp cannot be placed in the same hint sample.

Choose an RTP hint track time scale that provides adequate spacing between samples (as well as adequate spacing between transmission times for packets within a sample).

The packetization hint sample data contains the data elements listed in the following table.

| Packetization hint sample data | Bytes |
|----|----|
| Entry count | 2 |
| Reserved | 2 |
| Packet entry table | Variable |
| Additional data | Variable |

## Topics

### Data fields

Entry count

A 16-bit unsigned integer indicating the number of packet entries in the table.

Reserved

Two bytes.

Packet entry table

A variable length table containing packet entries.

Additional data

A variable length field containing data pointed to by the entries in the data table.

### Packet entries

Packet entry

A packet entry.

### Data modes

Data modes

Data formats you use in extra information TLVs.

## See Also

### Hint media

Hint media

Provide information about data units to stream in hint tracks.

Finding an original media track from a hint track

Use track reference atoms from hint tracks to locate the original media track.

RTP hint tracks

Allow a streaming server to create RTP streams from a QuickTime movie.

Hint track sample description

An atom that specifies the data format and location of the hint track sample data.

