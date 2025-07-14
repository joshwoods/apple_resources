

- UIKit
-  NSShadow 

Class

# NSShadow

An object you use to specify attributes to create and style a drop shadow during drawing operations.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSShadow
```

## Overview

When you create shadows, the system draws them in the default user coordinate space, where coordinates are independent from the pixel values of any particular device. Rotations, translations, and other transformations of the current transformation matrix (CTM) don’t affect the shadow or the apparent position of the shadow’s light source.

A shadow has two positional parameters: an x-offset and a y-offset. Express these values with a single size data type (CGSize in iOS, NSSize in macOS), using the units of the default user coordinate space. Positive values for these offsets extend down and to the right from the user’s perspective.

In addition to its positional parameters, a shadow also contains a blur radius, which specifies how much the system blurs a drawn object’s image mask before compositing the image onto the destination. A value of `0` produces no blur. Larger values produce an increasingly large blurred shadow.

You can use an NSShadow object in one of two ways. First, you can set it, like a color or a font, where `NSShadow` attributes apply to everything you draw until you apply another shadow or restore a previous graphics state. Second, you can use an `NSShadow` instance as the value for the the shadow text attribute in Swift or the NSShadowAttributeName text attribute in Objective-C, so the system applies the shadow to the glyphs corresponding to the characters bearing this attribute.

## Topics

### Creating a shadow

init()

Creates a shadow object with default values.

init?(coder: NSCoder)

Creates a shadow object from data in an unarchiver.

### Managing a shadow

var shadowOffset: CGSize

The shadow’s relative position, which you specify with horizontal and vertical offset values.

var shadowBlurRadius: CGFloat

The blur radius of the shadow.

var shadowColor: Any?

The color of the shadow.

### Setting a shadow

func set()

Sets the shadow of subsequent drawing operations to the current shadow.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

