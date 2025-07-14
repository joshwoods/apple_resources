

- RoomPlan
- RoomCaptureView
-  traitCollectionDidChange(\_:) 

Instance Method

# traitCollectionDidChange(\_:)

Notifies the view when the device orientation changes.

iOS 16.0+iPadOS 16.0+

``` source
@MainActor @preconcurrency
override dynamic func traitCollectionDidChange(_ previousTraitCollection: UITraitCollection?)
```

## Parameters 

`previousTraitCollection`  

The prior state of the trait collection before the change occurs.

## Overview

This property inherits from UIView.

## See Also

### Accessing view features

var subviews: [UIView]

An array that contains the view’s subviews.

func layoutSubviews()

Instructs the view’s subviews to position within the view.

func encode(with: NSCoder)

Serializes the view to the specified coder.

