

- UIKit
-  UIGraphicsImageRenderer 

Class

# UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsImageRenderer
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Overview

You can use image renderers to accomplish drawing tasks, without having to handle configuration such as color depth and image scale, or manage Core Graphics contexts. You initialize an image renderer with parameters such as image output dimensions and format. You then use one or more of the drawing functions to render images that share these properties.

To render an image:

1.  Optionally, create a UIGraphicsImageRendererFormat object to specify nondefault parameters the renderer should use to create its context.

2.  Instantiate a UIGraphicsImageRenderer object, providing the dimensions of the output image and a format object. The renderer uses default values for the current device if you don’t provide format object, as demonstrated in Creating a graphics image renderer.

3.  Choose one of the rendering methods depending on the output you desire: image(actions:) returns a UIImage object; jpegData(withCompressionQuality:actions:) returns a JPEG-encoded Data object; and pngData(actions:) returns a PNG-encoded Data object.

4.  Execute your chosen method, providing Core Graphics drawing instructions as the closure argument, as shown in Creating an image with an image renderer. Using blend mode demonstrates some of the more advanced rendering features you can use in your drawing instructions.

5.  Optionally, you can use Core Graphics drawing code within the drawing instructions you provide to the rendering method, as shown in Using Core Graphics rendering functions.

After initializing an image renderer, you can use it to draw multiple images with the same configuration. An image renderer keeps a cache of Core Graphics contexts, so reusing the same renderer can be more efficient than creating new renderers.

### Creating a graphics image renderer

Create an image renderer, providing the size of the output image:

- Swift
- Objective-C

```
let renderer = UIGraphicsImageRenderer(size: CGSize(width: 200, height: 200))
```

```
UIGraphicsImageRenderer *renderer = [[UIGraphicsImageRenderer alloc] initWithSize:CGSizeMake(200, 200)];
```

You can instead use one of the other UIGraphicsImageRenderer initializers to specify a renderer format (UIGraphicsImageRendererFormat) in addition to the size. This allows you to configure the underlying Core Graphics context for wide color and retina images.

If you don’t provide a format, the renderer uses the default() format, which creates a context best suited for the current device.

### Creating an image with an image renderer

Use the image(actions:) method to create an image (UIImage object) with an image renderer. This method takes a closure that represents the drawing actions. Within this closure, the renderer creates a Core Graphics context using the parameters provided during renderer initialization, and sets this Core Graphics context to be the current context.

- Swift
- Objective-C

```
let image = renderer.image { (context) in
  UIColor.darkGray.setStroke()
  context.stroke(renderer.format.bounds)
  UIColor(colorLiteralRed: 158/255, green: 215/255, blue: 245/255, alpha: 1).setFill()
  context.fill(CGRect(x: 1, y: 1, width: 140, height: 140))
}
```

```
  UIImage *image = [renderer imageWithActions:^(UIGraphicsImageRendererContext * _Nonnull context) {
    [[UIColor darkGrayColor] setStroke];
    [context strokeRect:renderer.format.bounds];
    [[UIColor colorWithRed:158/255.0 green:215/255.0 blue:245/255.0 alpha:1] setFill];
    [context fillRect:CGRectMake(1, 1, 140, 140)];
  }];
```

The drawing actions closure takes a single argument of type UIGraphicsImageRendererContext. This provides access to some high-level drawing functions, such as fill(_:), through the UIGraphicsRendererContext superclass.

The above code creates the following image:

In addition to the image(actions:) method that creates an UIImage object, UIGraphicsImageRenderer also has jpegData(withCompressionQuality:actions:) and pngData(actions:) methods that create Data objects containing the image encoded as a JPEG or a PNG respectively. All three methods take the same approach as detailed here, accepting a block that represents the drawing actions.

### Using blend mode

The utility methods on UIGraphicsImageRendererContext also offer a variant that accepts a CGBlendMode value. This value determines how to combine the pixel values when painting.

- Swift
- Objective-C

```
let image = renderer.image { (context) in
  UIColor.darkGray.setStroke()
  context.stroke(renderer.format.bounds)
  UIColor(colorLiteralRed: 158/255, green: 215/255, blue: 245/255, alpha: 1).setFill()
  context.fill(CGRect(x: 1, y: 1, width: 140, height: 140))
  UIColor(colorLiteralRed: 145/255, green: 211/255, blue: 205/255, alpha: 1).setFill()
  context.fill(CGRect(x: 60, y: 60, width: 140, height: 140), blendMode: .multiply)
}
```

```
  UIImage *image = [renderer imageWithActions:^(UIGraphicsImageRendererContext * _Nonnull context) {
    [[UIColor darkGrayColor] setStroke];
    [context strokeRect:renderer.format.bounds];
    [[UIColor colorWithRed:158/255.0 green:215/255.0 blue:245/255.0 alpha:1] setFill];
    [context fillRect:CGRectMake(1, 1, 140, 140)];
    [[UIColor colorWithRed:145/255.0 green:211/255.0 blue:205/255.0 alpha:1] setFill];
    [context fillRect:CGRectMake(60, 60, 140, 140) blendMode:kCGBlendModeMultiply];
  }];
```

This code draws a second square, using a blend mode of multiply. The following image shows the result.

### Using Core Graphics rendering functions

The UIGraphicsImageRendererContext available in the image closure has a cgContext property, which allows you to use Core Graphics rendering functions directly. For example, the following code demonstrates how to add a circle to the image:

- Swift
- Objective-C

```
let image = renderer.image { (context) in
  UIColor.darkGray.setStroke()
  context.stroke(renderer.format.bounds)
  UIColor(colorLiteralRed: 158/255, green: 215/255, blue: 245/255, alpha: 1).setFill()
  context.fill(CGRect(x: 1, y: 1, width: 140, height: 140))
  UIColor(colorLiteralRed: 145/255, green: 211/255, blue: 205/255, alpha: 1).setFill()
  context.fill(CGRect(x: 60, y: 60, width: 140, height: 140), blendMode: .multiply)

  UIColor(colorLiteralRed: 203/255, green: 222/255, blue: 116/255, alpha: 0.6).setFill()
  context.cgContext.fillEllipse(in: CGRect(x: 60, y: 60, width: 140, height: 140))
}
```

```
  UIImage *image = [renderer imageWithActions:^(UIGraphicsImageRendererContext * _Nonnull context) {
    [[UIColor darkGrayColor] setStroke];
    [context strokeRect:renderer.format.bounds];
    [[UIColor colorWithRed:158/255.0 green:215/255.0 blue:245/255.0 alpha:1] setFill];
    [context fillRect:CGRectMake(1, 1, 140, 140)];
    [[UIColor colorWithRed:145/255.0 green:211/255.0 blue:205/255.0 alpha:1] setFill];
    [context fillRect:CGRectMake(60, 60, 140, 140) blendMode:kCGBlendModeMultiply];

    [[UIColor colorWithRed:203/255.0 green:222/255.0 blue:116/255.0 alpha:0.6] setFill];
    CGContextFillEllipseInRect(context.CGContext, CGRectMake(60, 60, 140, 140));
  }];
```

This code uses the fillEllipse(in:) method on CGContext to draw a green circle on the blue and turquoise squares image; the following image shows the result.

## Topics

### Initializing an image renderer

init(bounds: CGRect, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified bounds and format.

convenience init(size: CGSize)

Creates an image renderer for drawing images of the specified size.

init(size: CGSize, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified size and format.

### Creating images

func image(actions: (UIGraphicsImageRendererContext) -> Void) -> UIImage

Creates an image from a set of drawing instructions.

func jpegData(withCompressionQuality: CGFloat, actions: (UIGraphicsImageRendererContext) -> Void) -> Data

Creates a JPEG-encoded image from a set of drawing instructions.

func pngData(actions: (UIGraphicsImageRendererContext) -> Void) -> Data

Creates a PNG-encoded image from a set of drawing instructions.

typealias DrawingActions

A closure for drawing an image.

## Relationships

### Inherits From

- UIGraphicsRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

