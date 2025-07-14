

- UIKit
-  UIGraphicsRenderer 

Class

# UIGraphicsRenderer

An abstract base class for creating graphics renderers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsRenderer
```

## Overview

Don’t use UIGraphicsRenderer directly. Instead, either use one of the concrete subclasses (UIGraphicsImageRenderer or UIGraphicsPDFRenderer), or create your own subclass.

Graphics renderers provide memory-efficient management of Core Graphics contexts. Core Graphics contexts represent the drawing environment and backing store for 2D Graphics. As you reuse a graphics renderer, it in turn reuses Core Graphics contexts.

### Subclassing notes

You can’t use UIGraphicsRenderer directly, but if the concrete subclasses (UIGraphicsPDFRenderer and UIGraphicsImageRenderer) don’t provide the functionality you require, you can create your own subclass.

Consider creating a subclass any time you need to create multiple Core Graphics contexts, each with the same dimensions and attributes, and one of the concrete subclasses (UIGraphicsPDFRenderer or UIGraphicsImageRenderer) doesn’t provide the functionality you require.

To create a subclass of UIGraphicsRenderer, first import the appropriate submodule or header, as shown in the following code.

- Swift
- Objective-C

```
import UIKit.UIGraphicsRendererSubclass
```

```
#import 
```

A graphics renderer manages a pool of Core Graphics contexts that are reused with repeated uses of the renderer. The renderer creates these CGContext objects using the context(with:) class method, and then wraps each of them in an instance of the class returned by the rendererContextClass() class method. You must therefore override these two methods in your graphics renderer subclass.

To perform drawing actions on a Core Graphics context, call the runDrawingActions(_:completionActions:) method, providing two blocks. Both of these blocks have a UIGraphicsRendererContext argument, providing access to a Core Graphics context.

It is recommended that you create a public method on your renderer subclass that internally wraps the runDrawingActions(_:completionActions:) method. This is how the rendering methods operate on the concrete subclasses, for example the image(actions:) method on UIGraphicsImageRenderer.

Each time the runDrawingActions(_:completionActions:) method is called, the renderer calls the prepare(_:with:) method with the CGContext and UIGraphicsRendererContext as arguments. Override the prepare(_:with:) method to apply the UIGraphicsRendererContext configuration to the underlying CGContext before the renderer invokes the drawing actions.

## Topics

### Initializing a graphics renderer

convenience init(bounds: CGRect)

Creates a new graphics renderer with the specified bounds and a default format.

init(bounds: CGRect, format: UIGraphicsRendererFormat)

Creates a new graphics renderer with the given bounds and format.

### Configuring the renderer

var allowsImageOutput: Bool

A Boolean value specifying whether the renderer can create output images.

var format: UIGraphicsRendererFormat

The format used to create the graphics renderer.

### Running the drawing actions

func runDrawingActions((UIGraphicsRendererContext) -> Void, completionActions: ((UIGraphicsRendererContext) -> Void)?) throws

Performs drawing actions on a Core Graphics context that the renderer prepares.

typealias UIGraphicsDrawingActions

A closure that executes a set of drawing instructions that the renderer applies to the Core Graphics context.

### Managing graphics contexts

class func context(with: UIGraphicsRendererFormat) -> CGContext?

Creates a Core Graphics context configured according to the supplied format object.

class func prepare(CGContext, with: UIGraphicsRendererContext)

Applies the configuration specified in the renderer context to the Core Graphics context.

class func rendererContextClass() -> AnyClass

Specifies the drawing context class used by this graphics renderer.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIGraphicsImageRenderer
- UIGraphicsPDFRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

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

