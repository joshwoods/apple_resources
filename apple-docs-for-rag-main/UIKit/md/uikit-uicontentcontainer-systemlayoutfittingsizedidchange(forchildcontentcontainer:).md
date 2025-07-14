

- UIKit
- UIContentContainer
-  systemLayoutFittingSizeDidChange(forChildContentContainer:) 

Instance Method

# systemLayoutFittingSizeDidChange(forChildContentContainer:)

Notifies the container that a child view controller was resized using Auto Layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func systemLayoutFittingSizeDidChange(forChildContentContainer container: any UIContentContainer)
```

**Required**

## Parameters 

`container`  

The child view controller that received the resizing message.

## Discussion

This method is called when a view controller that doesn’t use Auto Layout has a child view controller that uses Auto Layout and the child view controller is resized. When the child view controller responds to the systemLayoutSizeFitting(_:) method, the systemLayoutFittingSizeDidChange(forChildContentContainer:) method is sent to the parent view controller.

## See Also

### Responding to changes in child view controllers

func size(forChildContentContainer: any UIContentContainer, withParentContainerSize: CGSize) -> CGSize

Returns the size of the specified child view controller’s content.

**Required**

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies an interested controller that the preferred content size of one of its children changed.

**Required**

var preferredContentSize: CGSize

The preferred size for the container’s content.

**Required**

