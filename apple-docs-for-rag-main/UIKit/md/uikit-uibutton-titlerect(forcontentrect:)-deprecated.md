

- UIKit
- UIButton
-  titleRect(forContentRect:) Deprecated

Instance Method

# titleRect(forContentRect:)

Returns the rectangle in which the receiver draws its title.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 2.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func titleRect(forContentRect contentRect: CGRect) -> CGRect
```

## Parameters 

`contentRect`  

The content rectangle for the receiver.

## Return Value

The rectangle in which the receiver draws its title.

## See Also

### Dimensions

func backgroundRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its background.

Deprecated

func contentRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its entire content.

Deprecated

func imageRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its image.

Deprecated

