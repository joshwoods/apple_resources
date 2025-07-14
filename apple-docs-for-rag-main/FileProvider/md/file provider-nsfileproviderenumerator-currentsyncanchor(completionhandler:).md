

- File Provider
- NSFileProviderEnumerator
-  currentSyncAnchor(completionHandler:) 

Instance Method

# currentSyncAnchor(completionHandler:)

Returns the current sync anchor.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional func currentSyncAnchor(completionHandler: @escaping (NSFileProviderSyncAnchor?) -> Void)
```

``` source
optional func currentSyncAnchor() async -> NSFileProviderSyncAnchor?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func currentSyncAnchor() async -> NSFileProviderSyncAnchor?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Enumerating Items and Changes

func enumerateItems(for: any NSFileProviderEnumerationObserver, startingAt: NSFileProviderPage)

Requests the next batch of items, starting at the specified page.

**Required**

func enumerateChanges(for: any NSFileProviderChangeObserver, from: NSFileProviderSyncAnchor)

Requests the next batch of changes after the specified sync anchor.

func invalidate()

Stops the enumeration of items and changes.

**Required**

