

- Network
- NWConnection
-  requestEstablishmentReport(queue:completion:) 

Instance Method

# requestEstablishmentReport(queue:completion:)

Requests a copy of the connection’s establishment report once the connection is in the ready state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
final func requestEstablishmentReport(
    queue: DispatchQueue,
    completion: @escaping (NWConnection.EstablishmentReport?) -> Void
)
```

## See Also

### Collecting Connection Metrics

Collecting Network Connection Metrics

Use reports to understand how DNS and protocol handshakes impact connection establishment.

struct EstablishmentReport

A report that provides metrics about the establishment of a connection.

func startDataTransferReport() -> NWConnection.PendingDataTransferReport

Begins a new data transfer report, which can later be collected.

class PendingDataTransferReport

An outstanding data transfer report that has yet to be collected.

struct DataTransferReport

A report that provides metrics about data being sent and received on a connection.

