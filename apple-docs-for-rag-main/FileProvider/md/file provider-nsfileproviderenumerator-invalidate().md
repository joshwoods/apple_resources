

- File Provider
- NSFileProviderEnumerator
-  invalidate() 

Instance Method

# invalidate()

Stops the enumeration of items and changes.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func invalidate()
```

**Required**

## See Also

### Enumerating Items and Changes

func enumerateItems(for: any NSFileProviderEnumerationObserver, startingAt: NSFileProviderPage)

Requests the next batch of items, starting at the specified page.

**Required**

func enumerateChanges(for: any NSFileProviderChangeObserver, from: NSFileProviderSyncAnchor)

Requests the next batch of changes after the specified sync anchor.

func currentSyncAnchor(completionHandler: (NSFileProviderSyncAnchor?) -> Void)

Returns the current sync anchor.

