

- Network
- NWConnection
-  NWConnection.PendingDataTransferReport 

Class

# NWConnection.PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class PendingDataTransferReport
```

## Topics

### Collecting Reports

func collect(queue: DispatchQueue, completion: (NWConnection.DataTransferReport) -> Void)

Stops an outstanding data transfer report and delivers the result.

## Relationships

### Conforms To

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

struct DataTransferReport

A report that provides metrics about data being sent and received on a connection.

