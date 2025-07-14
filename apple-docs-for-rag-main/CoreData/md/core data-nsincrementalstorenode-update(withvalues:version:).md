

- Core Data
- NSIncrementalStoreNode
-  update(withValues:version:) 

Instance Method

# update(withValues:version:)

Update the values and version to reflect new data being saved to or loaded from the external store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func update(
    withValues values: [String : Any],
    version: UInt64
)
```

## Parameters 

`values`  

A dictionary containing updated values, in the same format as that described in init(objectID:withValues:version:).

`version`  

The version number for the transaction.

## Discussion

Update the values and version to reflect new data being saved to or loaded from the external store. // The values dictionary is in the same format as the initializer

## See Also

### Managing Node Data

var objectID: NSManagedObjectID

The object ID that identifies the data stored by the receiver.

func value(for: NSPropertyDescription) -> Any?

Returns the value for the given property.

var version: UInt64

The version of data in the receiver.

