

- UIKit
- UIColor
-  withAlphaComponent(\_:) 

Instance Method

# withAlphaComponent(\_:)

Creates a color object that has the same color space and component values as the receiver, but has the specified alpha component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func withAlphaComponent(_ alpha: CGFloat) -> UIColor
```

## Parameters 

`alpha`  

The opacity value of the new color object, specified as a value from 0.0 to 1.0. Alpha values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## Return Value

The new `UIColor` object.

## Discussion

A subclass with explicit opacity components should override this method to return a color with the specified alpha.

## See Also

### Creating a color from another color object

convenience init(Color)

Creates a color object that encapsulates a SwiftUI color.

init(ciColor: CIColor)

Creates a color object that encapsulates a Core Image color.

init(cgColor: CGColor)

Creates a color object using the specified Quartz color reference.

