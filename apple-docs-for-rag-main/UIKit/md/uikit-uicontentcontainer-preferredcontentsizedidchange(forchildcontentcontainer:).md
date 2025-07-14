

- UIKit
- UIContentContainer
-  preferredContentSizeDidChange(forChildContentContainer:) 

Instance Method

# preferredContentSizeDidChange(forChildContentContainer:)

Notifies an interested controller that the preferred content size of one of its children changed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func preferredContentSizeDidChange(forChildContentContainer container: any UIContentContainer)
```

**Required**

## Parameters 

`container`  

The child view controller whose preferred content size has changed.

## Discussion

UIKit calls this method on a container view controller when the preferredContentSize property of one of its child view controllers changes. Similarly, if the view controller is managed by a presentation controller, UIKit calls this method on the presentation controller to let it know of the change. The parent view controller or presentation controller can use this method to initiate layout adjustments based on the new size information.

## See Also

### Responding to changes in child view controllers

func size(forChildContentContainer: any UIContentContainer, withParentContainerSize: CGSize) -> CGSize

Returns the size of the specified child view controller’s content.

**Required**

func systemLayoutFittingSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies the container that a child view controller was resized using Auto Layout.

**Required**

var preferredContentSize: CGSize

The preferred size for the container’s content.

**Required**

