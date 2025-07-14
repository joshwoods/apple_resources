

- Core Data
- NSPersistentStoreCoordinator
-  persistentStore(for:) 

Instance Method

# persistentStore(for:)

Returns the persistent store for the specified file URL.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func persistentStore(for URL: URL) -> NSPersistentStore?
```

## Parameters 

`URL`  

An URL object that specifies the location of a persistent store.

## Return Value

The persistent store at the location specified by `URL`.

## See Also

### Managing a store’s location

func setURL(URL, for: NSPersistentStore) -> Bool

Changes the location of the specified persistent store.

func url(for: NSPersistentStore) -> URL

Returns the location of the provided persistent store.

