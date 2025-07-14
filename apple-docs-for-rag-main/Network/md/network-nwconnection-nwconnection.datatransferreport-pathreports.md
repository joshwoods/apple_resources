

- Network
- NWConnection
- NWConnection.DataTransferReport
-  pathReports 

Instance Property

# pathReports

An array of reports for each network path the connection used.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let pathReports: [NWConnection.DataTransferReport.PathReport]
```

## See Also

### Examining Data Transfer

let aggregatePathReport: NWConnection.DataTransferReport.PathReport

A report that sums counts across all network paths.

struct PathReport

A report that contains details about data transfer over a single network path.

