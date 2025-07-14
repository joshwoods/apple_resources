

- UIKit
- UIContentContainer
-  size(forChildContentContainer:withParentContainerSize:) 

Instance Method

# size(forChildContentContainer:withParentContainerSize:)

Returns the size of the specified child view controller’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func size(
    forChildContentContainer container: any UIContentContainer,
    withParentContainerSize parentSize: CGSize
) -> CGSize
```

**Required**

## Parameters 

`container`  

The child view controller.

`parentSize`  

The size of the parent view controller.

## Return Value

The size to apply to the child view controller.

## Discussion

Container view controllers use this method to return the sizes for their child view controllers. UIKit calls the method as part of the default implementation of the viewWillTransition(to:with:) method for view controllers. It calls the method once for each child view controller embedded in the view controller. If you’re implementing a custom container view controller, you should override this method and use it to return the sizes of the contained children.

View controllers and presentation controllers return the value in `parentSize` by default.

## See Also

### Responding to changes in child view controllers

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies an interested controller that the preferred content size of one of its children changed.

**Required**

func systemLayoutFittingSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies the container that a child view controller was resized using Auto Layout.

**Required**

var preferredContentSize: CGSize

The preferred size for the container’s content.

**Required**

