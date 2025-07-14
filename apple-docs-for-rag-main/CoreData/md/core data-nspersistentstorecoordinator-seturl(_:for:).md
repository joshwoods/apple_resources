

- Core Data
- NSPersistentStoreCoordinator
-  setURL(\_:for:) 

Instance Method

# setURL(\_:for:)

Changes the location of the specified persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setURL(
    _ url: URL,
    for store: NSPersistentStore
) -> Bool
```

## Parameters 

`url`  

The new location for `store`.

`store`  

A persistent store associated with the receiver.

## Return Value

true if the store was relocated, otherwise false.

## Discussion

For atomic stores, this method alters the location to which the next save operation will write the file; for non-atomic stores, invoking this method will relinquish the existing connection and create a new one at the specified URL. (For non-atomic stores, a store must already exist at the destination URL; a new store will not be created.)

## See Also

### Managing a store’s location

func persistentStore(for: URL) -> NSPersistentStore?

Returns the persistent store for the specified file URL.

func url(for: NSPersistentStore) -> URL

Returns the location of the provided persistent store.

