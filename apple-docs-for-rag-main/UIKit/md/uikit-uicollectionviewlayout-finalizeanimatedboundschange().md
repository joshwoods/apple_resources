

- UIKit
- UICollectionViewLayout
-  finalizeAnimatedBoundsChange() 

Instance Method

# finalizeAnimatedBoundsChange()

Cleans up after any animated changes to the view’s bounds or after the insertion or deletion of items.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func finalizeAnimatedBoundsChange()
```

## Discussion

The collection view calls this method after creating the animations for changing the view’s bounds or after the animated insertion or deletion of items. This method is the layout object’s opportunity to do any cleanup related to those operations.

You can also use this method to perform additional animations. Any animations you create are added to the animation block used to handle the insertions, deletions, and bounds changes.

## See Also

### Coordinating animated changes

func prepare(forAnimatedBoundsChange: CGRect)

Prepares the layout object for animated changes to the view’s bounds or the insertion or deletion of items.

