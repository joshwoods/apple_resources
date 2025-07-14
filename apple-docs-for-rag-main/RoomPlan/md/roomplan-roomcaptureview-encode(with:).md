

- RoomPlan
- RoomCaptureView
-  encode(with:) 

Instance Method

# encode(with:)

Serializes the view to the specified coder.

iOS 16.0+iPadOS 16.0+

``` source
@MainActor @preconcurrency
override dynamic func encode(with coder: NSCoder)
```

## Parameters 

`coder`  

An object that the view serializes to.

## Overview

This property inherits from UIView.

## See Also

### Accessing view features

var subviews: [UIView]

An array that contains the view’s subviews.

func layoutSubviews()

Instructs the view’s subviews to position within the view.

func traitCollectionDidChange(UITraitCollection?)

Notifies the view when the device orientation changes.

