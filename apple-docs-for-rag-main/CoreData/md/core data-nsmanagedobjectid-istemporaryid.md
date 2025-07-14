

- Core Data
- NSManagedObjectID
-  isTemporaryID 

Instance Property

# isTemporaryID

A Boolean value that indicates whether the object ID is temporary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isTemporaryID: Bool { get }
```

## Discussion

true if the receiver is temporary, otherwise false. Most object IDs return false. New objects inserted into a managed object context are assigned a temporary ID which is replaced with a permanent one once the object gets saved to a persistent store.

## See Also

### Getting Managed Object ID Information

var entity: NSEntityDescription

The entity description associated with the object ID.

var persistentStore: NSPersistentStore?

The persistent store that fetched the object for the object ID.

func uriRepresentation() -> URL

Returns a URI that provides an archiveable reference to the object for the object ID.

