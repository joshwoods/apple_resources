

- Core Data
- NSManagedObjectID
-  entity 

Instance Property

# entity

The entity description associated with the object ID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entity: NSEntityDescription { get }
```

## See Also

### Related Documentation

Core Data Programming Guide

var entity: NSEntityDescription

The entity description of the managed object.

### Getting Managed Object ID Information

var isTemporaryID: Bool

A Boolean value that indicates whether the object ID is temporary.

var persistentStore: NSPersistentStore?

The persistent store that fetched the object for the object ID.

func uriRepresentation() -> URL

Returns a URI that provides an archiveable reference to the object for the object ID.

