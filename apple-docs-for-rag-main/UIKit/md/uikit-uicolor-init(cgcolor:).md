

- UIKit
- UIColor
-  init(cgColor:) 

Initializer

# init(cgColor:)

Creates a color object using the specified Quartz color reference.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(cgColor: CGColor)
```

## Parameters 

`cgColor`  

A reference to a Quartz color.

## Return Value

An initialized color object. The color information represented by this object is in the native colorspace of the specified Quartz color.

## See Also

### Creating a color from another color object

convenience init(Color)

Creates a color object that encapsulates a SwiftUI color.

init(ciColor: CIColor)

Creates a color object that encapsulates a Core Image color.

func withAlphaComponent(CGFloat) -> UIColor

Creates a color object that has the same color space and component values as the receiver, but has the specified alpha component.

