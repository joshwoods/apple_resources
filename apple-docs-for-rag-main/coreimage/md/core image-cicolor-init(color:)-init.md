

- Core Image
- CIColor
-  init(color:) 

Initializer

# init(color:)

Initializes a Core Image color object using a UIKit (or AppKit) color object.

UIKitAppKitiOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
convenience init(color: UIColor)
```

**macOS**

``` source
convenience init?(color: NSColor)
```

## Parameters 

`color`  

The initial color value, which can belong to any available color space.

## Return Value

The resulting Core Image color, or (in macOS only) `nil` if the specified color cannot be converted.

## Discussion

In iOS and tvOS, this initializer takes a UIColor object and always returns a corresponding Core Image color object.

In macOS, this initializer takes an NSColor object. some possible NSColor configurations cannot be accurately represented as Core Image (or Core Graphics) colors—in such cases, this initializer returns `nil`.

## See Also

### Initializing Color Objects

init(cgColor: CGColor)

Initializes a Core Image color object with a Core Graphics color.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values.

init?(red: CGFloat, green: CGFloat, blue: CGFloat, colorSpace: CGColorSpace)

Initializes a Core Image color object with the specified red, green, and blue component values as measured in the specified color space.

init?(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat, colorSpace: CGColorSpace)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values as measured in the specified color space.

