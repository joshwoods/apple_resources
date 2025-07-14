

- UIKit
- UIColor
-  init(ciColor:) 

Initializer

# init(ciColor:)

Creates a color object that encapsulates a Core Image color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
init(ciColor: CIColor)
```

## Parameters 

`ciColor`  

The Core Image color to convert.

## Return Value

An initialized color object.

## See Also

### Creating a color from another color object

convenience init(Color)

Creates a color object that encapsulates a SwiftUI color.

init(cgColor: CGColor)

Creates a color object using the specified Quartz color reference.

func withAlphaComponent(CGFloat) -> UIColor

Creates a color object that has the same color space and component values as the receiver, but has the specified alpha component.

