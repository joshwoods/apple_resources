

- Network Extension
- NEFilterFlow
-  sourceAppIdentifier 

Instance Property

# sourceAppIdentifier

A string containing the identifier of the source app of the flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var sourceAppIdentifier: String? { get }
```

## Discussion

This identifier remains the same for all versions and builds of the app and is unique among all apps.

## See Also

### Source app identification

var sourceAppUniqueIdentifier: Data?

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

var sourceAppVersion: String?

The short version string of the app that is the source of the flow.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

var sourceProcessAuditToken: Data?

The audit token of the process that created the flow.

