

- File Provider
- NSFileProviderEnumerator
-  enumerateChanges(for:from:) 

Instance Method

# enumerateChanges(for:from:)

Requests the next batch of changes after the specified sync anchor.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional func enumerateChanges(
    for observer: any NSFileProviderChangeObserver,
    from syncAnchor: NSFileProviderSyncAnchor
)
```

## Mentioned in 

Tracking Changes to Documents

Signaling Changes for User-Driven Actions

## Discussion

The system requests an enumerator in the following situations:

- **For directories.** The system requests an enumerator when a document browser displays the contents of a directory. For performance reasons, the system may retain the enumerator even after the browser has moved to a different directory.

- **For files.** The system requests an enumerator when a file presenter begins managing an item. The enumerator is invalidated after the file presenter is removed.

- **For the working set.** The system requests an enumerator when it begins indexing the working set. It invalidates the enumerator after the indexing operation has completed.

Once requested, an enumerator is used to provide both the content and any changes for an item. When the system is finished with the item, it calls the enumerator’s invalidate() method. For example, if you return an enumerator that provides the content of a directory, as long as the enumerator is active, the system also uses it to enumerate changes to the directory.

The system may have multiple, active enumerators for a number of different items. Some of these may represent items that are currently displayed on screen. Others may be items that are no longer displayed, but the enumerator is retained for performance reasons. You need to inform the system of any changes to the content managed by any of the active enumerators, as well as any changes to the working set (whether or not it has an active enumerator).

For more information on enumerating items, see Defining Your File Provider’s Content. For more information on tracking changes, see Tracking Your File Provider’s Changes.

## See Also

### Enumerating Items and Changes

func enumerateItems(for: any NSFileProviderEnumerationObserver, startingAt: NSFileProviderPage)

Requests the next batch of items, starting at the specified page.

**Required**

func currentSyncAnchor(completionHandler: (NSFileProviderSyncAnchor?) -> Void)

Returns the current sync anchor.

func invalidate()

Stops the enumeration of items and changes.

**Required**

