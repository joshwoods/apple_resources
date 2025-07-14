

- UIKit
- UIContentContainer
-  preferredContentSize 

Instance Property

# preferredContentSize

The preferred size for the container’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredContentSize: CGSize { get }
```

**Required**

## Discussion

The UIViewController class implements a writable version of this property.

## See Also

### Responding to changes in child view controllers

func size(forChildContentContainer: any UIContentContainer, withParentContainerSize: CGSize) -> CGSize

Returns the size of the specified child view controller’s content.

**Required**

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies an interested controller that the preferred content size of one of its children changed.

**Required**

func systemLayoutFittingSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies the container that a child view controller was resized using Auto Layout.

**Required**

