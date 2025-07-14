

- AppKit
- NSCollectionViewLayout
-  finalizeAnimatedBoundsChange() 

Instance Method

# finalizeAnimatedBoundsChange()

Cleans up after any animated changes to the collection view’s bounds or after the insertion or deletion of items.

macOS

``` source
@MainActor
func finalizeAnimatedBoundsChange()
```

## Discussion

The default implementation of this method does nothing. The collection view calls this method after creating the animations for changing inserting or deleting items or for changing the collection view’s bounds. Subclasses can use this method to perform any cleanup operations related to those changes. You can also use this method to perform custom animations. Any animations you create are added to the animation block used to handle the insertions, deletions, and bounds changes.

## See Also

### Coordinating Animated Changes

func prepare(forAnimatedBoundsChange: NSRect)

Prepares the layout object for animated changes to the collection view’s bounds or for the insertion or deletion of items.

