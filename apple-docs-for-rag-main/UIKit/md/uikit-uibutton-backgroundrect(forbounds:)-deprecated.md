

- UIKit
- UIButton
-  backgroundRect(forBounds:) Deprecated

Instance Method

# backgroundRect(forBounds:)

Returns the rectangle in which the receiver draws its background.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 2.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func backgroundRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The bounds rectangle in which to draw any standard button content.

## Discussion

The default implementation of this method returns the value in the `bounds` parameter. This rectangle represents the area in which the button draws its standard background content. Subclasses that provide custom background adornments can override this method and return a modified bounds rectangle to prevent the button from drawing over any custom content.

## See Also

### Dimensions

func contentRect(forBounds: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its entire content.

Deprecated

func titleRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its title.

Deprecated

func imageRect(forContentRect: CGRect) -> CGRect

Returns the rectangle in which the receiver draws its image.

Deprecated

