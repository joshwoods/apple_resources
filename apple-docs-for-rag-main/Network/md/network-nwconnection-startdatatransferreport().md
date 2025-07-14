

- Network
- NWConnection
-  startDataTransferReport() 

Instance Method

# startDataTransferReport()

Begins a new data transfer report, which can later be collected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func startDataTransferReport() -> NWConnection.PendingDataTransferReport
```

## See Also

### Collecting Connection Metrics

Collecting Network Connection Metrics

Use reports to understand how DNS and protocol handshakes impact connection establishment.

func requestEstablishmentReport(queue: DispatchQueue, completion: (NWConnection.EstablishmentReport?) -> Void)

Requests a copy of the connection’s establishment report once the connection is in the ready state.

struct EstablishmentReport

A report that provides metrics about the establishment of a connection.

class PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

struct DataTransferReport

A report that provides metrics about data being sent and received on a connection.

