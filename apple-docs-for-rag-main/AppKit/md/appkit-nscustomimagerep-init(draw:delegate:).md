

- AppKit
- NSCustomImageRep
-  init(draw:delegate:) 

Initializer

# init(draw:delegate:)

Returns a representation of an image initialized with the specified delegate information.

macOS

``` source
init(
    draw selector: Selector,
    delegate: Any
)
```

## Parameters 

`selector`  

The selector to call when it is time to draw the image. The method should take a single parameter of type `id` that represents the NSCustomImageRep object that initiated drawing. The method must draw the image starting at the point (0, 0) in the current coordinate system.

`delegate`  

The delegate object that responds to the selector in `aMethod`.

## Return Value

An initialized NSCustomImageRep object, or `nil` if the object could not be initialized.

## Discussion

When the receiver is asked to draw the image, it sends the specified message to the selector, passing itself as a parameter to the delegate method. The delegate’s drawing method should have the following form:

```
- (void)myCustomDrawMethod:(id)anNSCustomImageRep;
```

## See Also

### Related Documentation

Cocoa Drawing Guide

func draw() -> Bool

Implemented by subclasses to draw the image in the current coordinate system.

### Creating Representations of Images in Custom Formats

init(size: NSSize, flipped: Bool, drawingHandler: (NSRect) -> Bool)

Initializes a representation of an image of the specified size and flipped status, using a block to draw its content.

