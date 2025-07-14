

- Core Data
- NSPersistentStoreCoordinator
-  managedObjectID(forURIRepresentation:) 

Instance Method

# managedObjectID(forURIRepresentation:)

Returns the object identifier for the specified URI representation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func managedObjectID(forURIRepresentation url: URL) -> NSManagedObjectID?
```

## Parameters 

`url`  

An URL object containing a URI that specify a managed object.

## Return Value

An object ID for the object specified by `url`.

## Discussion

The URI representation contains a UUID of the store the ID is coming from, and the coordinator can match it against the stores added to it.

## See Also

### Related Documentation

func object(with: NSManagedObjectID) -> NSManagedObject

Returns either an existing object from the context or a fault that represents that object.

func uriRepresentation() -> URL

Returns a URI that provides an archiveable reference to the object for the object ID.

