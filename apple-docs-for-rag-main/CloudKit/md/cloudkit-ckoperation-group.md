

- CloudKit
- CKOperation
-  group 

Instance Property

# group

The operation’s group.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var group: CKOperationGroup? { get set }
```

## See Also

### Managing the Operation’s Configuration

var configuration: CKOperation.Configuration!

The operation’s configuration.

class Configuration

An object that describes how a CloudKit operation behaves.

var longLivedOperationWasPersistedBlock: (() -> Void)?

The closure to execute when the server begins to store callbacks for the long-lived operation.

