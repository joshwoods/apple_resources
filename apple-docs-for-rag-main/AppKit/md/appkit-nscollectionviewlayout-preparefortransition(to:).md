

- AppKit
- NSCollectionViewLayout
-  prepareForTransition(to:) 

Instance Method

# prepareForTransition(to:)

Prepares the layout object to be uninstalled from the collection view.

macOS

``` source
@MainActor
func prepareForTransition(to newLayout: NSCollectionViewLayout)
```

## Parameters 

`newLayout`  

The layout object to install in the collection view at the end of the transition.

## Discussion

Prior to transitioning to a new layout object, the collection view calls this method on the old layout object to give it time to perform any cleanup operations.

## See Also

### Transitioning Between Layouts

func prepareForTransition(from: NSCollectionViewLayout)

Prepares the layout object to be installed in the collection view.

func finalizeLayoutTransition()

Performs any final steps related to a layout transition before the transition animations actually occur.

