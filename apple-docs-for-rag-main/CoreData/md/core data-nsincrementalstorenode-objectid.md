

- Core Data
- NSIncrementalStoreNode
-  objectID 

Instance Property

# objectID

The object ID that identifies the data stored by the receiver.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var objectID: NSManagedObjectID { get }
```

## See Also

### Managing Node Data

func update(withValues: [String : Any], version: UInt64)

Update the values and version to reflect new data being saved to or loaded from the external store.

func value(for: NSPropertyDescription) -> Any?

Returns the value for the given property.

var version: UInt64

The version of data in the receiver.

