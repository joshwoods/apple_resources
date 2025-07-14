

- UIKit
- UIButton
-  contentRect(forBounds:) Deprecated

Instance Method

# contentRect(forBounds:)

Returns the rectangle in which the receiver draws its entire content.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 2.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func contentRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle for the receiver.

## Return Value

The rectangle in which the receiver draws its entire content.

## Discussion

The content rectangle is the area needed to display the image and title including any padding and adjustments for alignment and other settings.

## See Also

### Related Documentation

var contentEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle surrounding all of the button’s content.

Deprecated

### Dimensions

func backgroundRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its background.

Deprecated

func titleRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its title.

Deprecated

func imageRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its image.

Deprecated

