

- SwiftData
- PersistentIdentifier
-  entityName 

Instance Property

# entityName

The entity name for the associated model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var entityName: String { get }
```

## See Also

### Accessing identity information

let id: PersistentIdentifier.ID

The value that uniquely identifies the associated model within the containing store.

struct ID

A type that represents the stable identity of a SwiftData model.

var storeIdentifier: String?

The identifier of the store that contains the associated model.

