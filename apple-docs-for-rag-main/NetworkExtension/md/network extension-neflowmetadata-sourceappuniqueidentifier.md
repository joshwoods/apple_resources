

- Network Extension
- NEFlowMetaData
-  sourceAppUniqueIdentifier 

Instance Property

# sourceAppUniqueIdentifier

A data instance that contains a unique hash value for the source application.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var sourceAppUniqueIdentifier: Data { get }
```

## Discussion

The property contains the Code Directory Hash for the application.

Note

The property’s value changes between different versions of an application.

## See Also

### Getting source app information

var sourceAppSigningIdentifier: String

A string that contains the signing identifier of the source application.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

