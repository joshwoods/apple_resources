

- UIKit
- UIInputView
-  init(frame:inputViewStyle:) 

Initializer

# init(frame:inputViewStyle:)

Initializes and returns an input view using the specified style information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    frame: CGRect,
    inputViewStyle: UIInputView.Style
)
```

## Parameters 

`frame`  

The frame rectangle for the view, measured in points. The origin of the frame is relative to the superview in which you plan to add it.

`inputViewStyle`  

The style to use when altering the appearance of the view and its subviews. For a list of possible values, see UIInputView.Style

## Return Value

An initialized view object or `nil` if the view could not be initialized.

## Discussion

This method is the designated initializer for the view and must be called by your subclass at initialization time.

## See Also

### Initializing an input view

init?(coder: NSCoder)

Creates an input view from data in an unarchiver.

