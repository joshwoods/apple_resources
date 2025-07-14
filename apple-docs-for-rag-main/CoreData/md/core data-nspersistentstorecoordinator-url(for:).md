

- Core Data
- NSPersistentStoreCoordinator
-  url(for:) 

Instance Method

# url(for:)

Returns the location of the provided persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func url(for store: NSPersistentStore) -> URL
```

## Parameters 

`store`  

A persistent store.

## Return Value

The URL for `store`.

## See Also

### Related Documentation

var persistentStores: [NSPersistentStore]

The coordinator’s persistent stores.

### Managing a store’s location

func setURL(URL, for: NSPersistentStore) -> Bool

Changes the location of the specified persistent store.

func persistentStore(for: URL) -> NSPersistentStore?

Returns the persistent store for the specified file URL.

