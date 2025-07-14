

- Foundation
- NSUbiquitousKeyValueStore
-  removeObject(forKey:) 

Instance Method

# removeObject(forKey:)

Removes the value associated with the specified key from the key-value store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func removeObject(forKey aKey: String)
```

## Parameters 

`aKey`  

The key corresponding to the value you want to remove.

## Discussion

If the specified key is not found in the key-value store, this method does nothing. This method removes the key from the in-memory version of the store only. Call the synchronize method at appropriate times to update the information on disk.

