

- Core Data
- NSIncrementalStoreNode
-  value(for:) 

Instance Method

# value(for:)

Returns the value for the given property.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func value(for prop: NSPropertyDescription) -> Any?
```

## Parameters 

`prop`  

A property description for one of the properties in the receiver.

## Return Value

The value for the property specified by `prop`. May return an instance of `NSNull` for to-one relationships.

## Discussion

If a relationship is `nil`, you should create a new value by invoking `newValueForRelationship:forObjectWithID:withContext:error:` on the `NSPersistentStore` object.

## See Also

### Managing Node Data

var objectID: NSManagedObjectID

The object ID that identifies the data stored by the receiver.

func update(withValues: [String : Any], version: UInt64)

Update the values and version to reflect new data being saved to or loaded from the external store.

var version: UInt64

The version of data in the receiver.

