

- Network
- NWConnection
-  NWConnection.DataTransferReport 

Structure

# NWConnection.DataTransferReport

A report that provides metrics about data being sent and received on a connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct DataTransferReport
```

## Topics

### Examining Data Transfer

let aggregatePathReport: NWConnection.DataTransferReport.PathReport

A report that sums counts across all network paths.

let pathReports: [NWConnection.DataTransferReport.PathReport]

An array of reports for each network path the connection used.

struct PathReport

A report that contains details about data transfer over a single network path.

### Summarizing Reports

let duration: TimeInterval

The duration of the data transfer report, from when it was started to when it was collected.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Collecting Connection Metrics

Collecting Network Connection Metrics

Use reports to understand how DNS and protocol handshakes impact connection establishment.

func requestEstablishmentReport(queue: DispatchQueue, completion: (NWConnection.EstablishmentReport?) -> Void)

Requests a copy of the connection’s establishment report once the connection is in the ready state.

struct EstablishmentReport

A report that provides metrics about the establishment of a connection.

func startDataTransferReport() -> NWConnection.PendingDataTransferReport

Begins a new data transfer report, which can later be collected.

class PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

