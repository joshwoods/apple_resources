

- CloudKit
- CKOperation
-  configuration 

Instance Property

# configuration

The operation’s configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@NSCopying
var configuration: CKOperation.Configuration! { get set }
```

## See Also

### Managing the Operation’s Configuration

class Configuration

An object that describes how a CloudKit operation behaves.

var group: CKOperationGroup?

The operation’s group.

var longLivedOperationWasPersistedBlock: (() -> Void)?

The closure to execute when the server begins to store callbacks for the long-lived operation.

