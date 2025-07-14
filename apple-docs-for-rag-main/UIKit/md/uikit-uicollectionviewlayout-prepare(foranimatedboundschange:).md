

- UIKit
- UICollectionViewLayout
-  prepare(forAnimatedBoundsChange:) 

Instance Method

# prepare(forAnimatedBoundsChange:)

Prepares the layout object for animated changes to the view’s bounds or the insertion or deletion of items.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func prepare(forAnimatedBoundsChange oldBounds: CGRect)
```

## Parameters 

`oldBounds`  

The current bounds of the collection view.

## Discussion

The collection view calls this method before performing any animated changes to the view’s bounds or before the animated insertion or deletion of items. This method is the layout object’s opportunity to perform any calculations needed to prepare for those animated changes. Specifically, you might use this method to calculate the initial or final positions of inserted or deleted items so that you can return those values when asked for them.

You can also use this method to perform additional animations. Any animations you create are added to the animation block used to handle the insertions, deletions, and bounds changes.

## See Also

### Coordinating animated changes

func finalizeAnimatedBoundsChange()

Cleans up after any animated changes to the view’s bounds or after the insertion or deletion of items.

