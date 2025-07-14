

- Network Extension
- NEFlowMetaData
-  sourceAppSigningIdentifier 

Instance Property

# sourceAppSigningIdentifier

A string that contains the signing identifier of the source application.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var sourceAppSigningIdentifier: String { get }
```

## Discussion

For all apps that are signed in the standard way using Xcode, this value is identical to the app’s bundle identifier.

## See Also

### Getting source app information

var sourceAppUniqueIdentifier: Data

A data instance that contains a unique hash value for the source application.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

