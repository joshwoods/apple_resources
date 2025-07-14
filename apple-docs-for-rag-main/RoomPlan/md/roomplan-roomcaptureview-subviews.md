

- RoomPlan
- RoomCaptureView
-  subviews 

Instance Property

# subviews

An array that contains the view’s subviews.

iOS 16.0+iPadOS 16.0+

``` source
@MainActor @preconcurrency
override dynamic var subviews: [UIView] { get }
```

## Overview

This property inherits from UIView.

## See Also

### Accessing view features

func layoutSubviews()

Instructs the view’s subviews to position within the view.

func encode(with: NSCoder)

Serializes the view to the specified coder.

func traitCollectionDidChange(UITraitCollection?)

Notifies the view when the device orientation changes.

