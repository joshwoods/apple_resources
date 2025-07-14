

- Network
- NWConnection
-  Collecting Network Connection Metrics 

Sample Code

# Collecting Network Connection Metrics

Use reports to understand how DNS and protocol handshakes impact connection establishment.

Download

iOS 13.0+iPadOS 13.0+Xcode 13.0+

## Overview

Note

This sample code project is associated with WWDC 2019 session 713: Advances in Networking, Part 2.

## See Also

### Collecting Connection Metrics

func requestEstablishmentReport(queue: DispatchQueue, completion: (NWConnection.EstablishmentReport?) -> Void)

Requests a copy of the connection’s establishment report once the connection is in the ready state.

struct EstablishmentReport

A report that provides metrics about the establishment of a connection.

func startDataTransferReport() -> NWConnection.PendingDataTransferReport

Begins a new data transfer report, which can later be collected.

class PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

struct DataTransferReport

A report that provides metrics about data being sent and received on a connection.

