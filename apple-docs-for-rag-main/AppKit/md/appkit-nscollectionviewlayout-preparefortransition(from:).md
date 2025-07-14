

- AppKit
- NSCollectionViewLayout
-  prepareForTransition(from:) 

Instance Method

# prepareForTransition(from:)

Prepares the layout object to be installed in the collection view.

macOS

``` source
@MainActor
func prepareForTransition(from oldLayout: NSCollectionViewLayout)
```

## Parameters 

`oldLayout`  

The layout object installed in the collection view at the beginning of the transition. You might use this object to retrieve the current layout attributes for items and views.

## Discussion

Prior to transitioning to a new layout object, the collection view calls this method on the new layout object to give it time to perform any initial calculations.

## See Also

### Transitioning Between Layouts

func prepareForTransition(to: NSCollectionViewLayout)

Prepares the layout object to be uninstalled from the collection view.

func finalizeLayoutTransition()

Performs any final steps related to a layout transition before the transition animations actually occur.

