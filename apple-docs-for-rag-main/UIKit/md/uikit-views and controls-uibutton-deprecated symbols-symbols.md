

- UIKit
- Views and controls
- UIButton
-  Deprecated symbols 

API Collection

# Deprecated symbols

Symbols that buttons no longer support.

## Topics

### Title effects

var reversesTitleShadowWhenHighlighted: Bool

A Boolean value that determines whether the title shadow changes when the button is highlighted.

Deprecated

### Button presentation

var adjustsImageWhenHighlighted: Bool

A Boolean value that determines whether the image changes when the button is highlighted.

Deprecated

var adjustsImageWhenDisabled: Bool

A Boolean value that determines whether the image changes when the button is disabled.

Deprecated

var showsTouchWhenHighlighted: Bool

A Boolean value that determines whether tapping the button causes it to glow.

Deprecated

### Edge insets

var contentEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle surrounding all of the button’s content.

Deprecated

var titleEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle around the button’s title text.

Deprecated

var imageEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle around the button’s image.

Deprecated

### Dimensions

func backgroundRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its background.

Deprecated

func contentRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its entire content.

Deprecated

func titleRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its title.

Deprecated

func imageRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its image.

Deprecated

