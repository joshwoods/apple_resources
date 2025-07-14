

- UIKit
- UICollectionViewTransitionLayout
-  init(currentLayout:nextLayout:) 

Initializer

# init(currentLayout:nextLayout:)

Initializes and returns a transition layout object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    currentLayout: UICollectionViewLayout,
    nextLayout newLayout: UICollectionViewLayout
)
```

## Parameters 

`currentLayout`  

The layout object currently in use by the collection view.

`newLayout`  

The new layout object that is being installed into the collection view.

## Return Value

An initialized transition layout object or `nil` if the object could not be created.

## Discussion

This method initializes the transition layout object and saves references to the current and new layout objects so that you can access them later. If you subclass and implement your own initialization method, you must call this method to initialize the superclass.

## See Also

### Initializing the transition layout object

init?(coder: NSCoder)

Creates a transition layout object from data in an unarchiver.

