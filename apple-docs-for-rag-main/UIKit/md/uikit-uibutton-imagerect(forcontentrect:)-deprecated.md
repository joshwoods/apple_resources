

- UIKit
- UIButton
-  imageRect(forContentRect:) Deprecated

Instance Method

# imageRect(forContentRect:)

Returns the rectangle in which the receiver draws its image.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 2.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func imageRect(forContentRect contentRect: CGRect) -> CGRect
```

## Parameters 

`contentRect`  

The content rectangle for the receiver.

## Return Value

The rectangle in which the receiver draws its image.

## See Also

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

