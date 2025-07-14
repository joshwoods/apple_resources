

- Network Extension
- NEFilterFlow
-  sourceAppAuditToken 

Instance Property

# sourceAppAuditToken

The audit token of the source application of the flow.

macOS 10.15+

``` source
var sourceAppAuditToken: Data? { get }
```

## See Also

### Source app identification

var sourceAppUniqueIdentifier: Data?

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

var sourceAppIdentifier: String?

A string containing the identifier of the source app of the flow.

var sourceAppVersion: String?

The short version string of the app that is the source of the flow.

var sourceProcessAuditToken: Data?

The audit token of the process that created the flow.

