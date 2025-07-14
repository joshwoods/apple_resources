

- AppKit
- NSCollectionViewLayout
-  prepare(forAnimatedBoundsChange:) 

Instance Method

# prepare(forAnimatedBoundsChange:)

Prepares the layout object for animated changes to the collection view’s bounds or for the insertion or deletion of items.

macOS

``` source
@MainActor
func prepare(forAnimatedBoundsChange oldBounds: NSRect)
```

## Parameters 

`oldBounds`  

The current bounds of the collection view.

## Discussion

The default implementation of this method does nothing. The collection view calls this method before performing any animated changes to the collection view’s bounds. It also calls this method before the animated insertion or deletion of items. Subclasses can use this method to perform any calculations needed to prepare for animated changes. Specifically, you might use this method to calculate the initial or final positions of inserted or deleted items so that you can return those values when asked for them. You can also use this method to perform custom animations. Any animations you create are added to the animation block used to handle the insertions, deletions, and bounds changes.

## See Also

### Coordinating Animated Changes

func finalizeAnimatedBoundsChange()

Cleans up after any animated changes to the collection view’s bounds or after the insertion or deletion of items.

