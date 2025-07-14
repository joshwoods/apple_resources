

- Core Data
- NSManagedObjectID
-  uriRepresentation() 

Instance Method

# uriRepresentation()

Returns a URI that provides an archiveable reference to the object for the object ID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func uriRepresentation() -> URL
```

## Return Value

An `NSURL` object containing a URI that provides an archiveable reference to the object which the receiver represents.

## Discussion

If the corresponding managed object has not yet been saved, the object ID (and hence URI) is a temporary value that will change when the corresponding managed object is saved.

## See Also

### Related Documentation

func managedObjectID(forURIRepresentation: URL) -> NSManagedObjectID?

Returns the object identifier for the specified URI representation.

func object(with: NSManagedObjectID) -> NSManagedObject

Returns either an existing object from the context or a fault that represents that object.

### Getting Managed Object ID Information

var entity: NSEntityDescription

The entity description associated with the object ID.

var isTemporaryID: Bool

A Boolean value that indicates whether the object ID is temporary.

var persistentStore: NSPersistentStore?

The persistent store that fetched the object for the object ID.

