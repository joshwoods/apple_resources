

- UIKit
- UICollectionViewLayout
-  prepareForTransition(from:) 

Instance Method

# prepareForTransition(from:)

Tells the layout object to prepare to be installed as the layout for the collection view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func prepareForTransition(from oldLayout: UICollectionViewLayout)
```

## Parameters 

`oldLayout`  

The layout object installed in the collection view at the beginning of the transition. You might use this object to provide different ending attributes based on the starting layout object.

## Discussion

Prior to performing a layout transition, the collection view calls this method so that your layout object can perform any initial calculations needed to generate layout attributes.

## See Also

### Transitioning between layouts

func prepareForTransition(to: UICollectionViewLayout)

Tells the layout object that it is about to be removed as the layout for the collection view.

func finalizeLayoutTransition()

Tells the layout object to perform any final steps before the transition animations occur.

