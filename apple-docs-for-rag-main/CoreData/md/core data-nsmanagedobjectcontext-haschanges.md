

- Core Data
- NSManagedObjectContext
-  hasChanges 

Instance Property

# hasChanges

A Boolean value that indicates whether the context has uncommitted changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var hasChanges: Bool { get }
```

## Discussion

If you are observing this property using key-value observing (KVO) you should not touch the context or its objects within your implementation of observeValue(forKeyPath:of:change:context:) for this notification. (This is because of the intricacy of the locations of the KVO notifications—for example, the context may be in the middle of an undo operation, or repairing a merge conflict.) If you need to send messages to the context or change any of its managed objects as a result of a change to the value of `hasChanges`, you must do so after the call stack unwinds (typically using perform(_:with:afterDelay:) or a similar method).

### Special Considerations

In macOS 10.6 and later, this property is Key-value observing compliant.

## See Also

### Managing unsaved and uncommitted changes

func save() throws

Attempts to commit unsaved changes to registered objects to the context’s parent store.

