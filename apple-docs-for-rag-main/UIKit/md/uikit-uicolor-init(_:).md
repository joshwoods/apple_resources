

- UIKit
- UIColor
-  init(\_:) 

Initializer

# init(\_:)

Creates a color object that encapsulates a SwiftUI color.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init(_ color: Color)
```

## Parameters 

`color`  

The initial color value, which can belong to any available color space.

## See Also

### Creating a color from another color object

init(ciColor: CIColor)

Creates a color object that encapsulates a Core Image color.

init(cgColor: CGColor)

Creates a color object using the specified Quartz color reference.

func withAlphaComponent(CGFloat) -> UIColor

Creates a color object that has the same color space and component values as the receiver, but has the specified alpha component.

