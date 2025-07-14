

- Core Data
- NSManagedObjectID
-  persistentStore 

Instance Property

# persistentStore

The persistent store that fetched the object for the object ID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
weak var persistentStore: NSPersistentStore? { get }
```

## Discussion

`nil` if the ID is for a newly-inserted object that has not yet been saved to a persistent store.

## See Also

### Getting Managed Object ID Information

var entity: NSEntityDescription

The entity description associated with the object ID.

var isTemporaryID: Bool

A Boolean value that indicates whether the object ID is temporary.

func uriRepresentation() -> URL

Returns a URI that provides an archiveable reference to the object for the object ID.

