

- Network Extension
- NEFilterFlow
-  sourceProcessAuditToken 

Instance Property

# sourceProcessAuditToken

The audit token of the process that created the flow.

macOS 13.0+

``` source
var sourceProcessAuditToken: Data? { get }
```

## Discussion

In cases where a system process creates the connection on behalf of a source app, this value is different from sourceAppAuditToken. In cases where the source app directly creates the connection, these values are identical.

## See Also

### Source app identification

var sourceAppUniqueIdentifier: Data?

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

var sourceAppIdentifier: String?

A string containing the identifier of the source app of the flow.

var sourceAppVersion: String?

The short version string of the app that is the source of the flow.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

