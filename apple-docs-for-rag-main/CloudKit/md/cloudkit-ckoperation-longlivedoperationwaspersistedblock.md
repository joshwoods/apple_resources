

- CloudKit
- CKOperation
-  longLivedOperationWasPersistedBlock 

Instance Property

# longLivedOperationWasPersistedBlock

The closure to execute when the server begins to store callbacks for the long-lived operation.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 9.2+visionOS 1.0+watchOS 3.0+

``` source
var longLivedOperationWasPersistedBlock: (() -> Void)? { get set }
```

## Discussion

If your app exits before CloudKit calls this property’s value, the system doesn’t include the operation’s ID in the results of calls to the fetchAllLongLivedOperationIDsWithCompletionHandler: method.

For more information, see Long-Lived Operations.

## See Also

### Managing the Operation’s Configuration

var configuration: CKOperation.Configuration!

The operation’s configuration.

class Configuration

An object that describes how a CloudKit operation behaves.

var group: CKOperationGroup?

The operation’s group.

