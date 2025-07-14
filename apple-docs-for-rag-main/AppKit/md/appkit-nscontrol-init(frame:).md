

- AppKit
- NSControl
-  init(frame:) 

Initializer

# init(frame:)

Initializes a control with the specified frame rectangle.

macOS

``` source
@MainActor
init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The rectangle of the control, specified in points in the coordinate space of the enclosing view.

## Return Value

An initialized control object, or `nil` if the object couldn’t be initialized.

## Discussion

If a cell has been specified for controls of this type, this method also creates an instance of the cell. Because `NSControl` is an abstract class, invocations of this method should appear only in the designated initializers of subclasses; that is, there should always be a more specific designated initializer for the subclass, as this method is the designated initializer for `NSControl`.

## See Also

### Related Documentation

Control and Cell Programming Topics

### Creating a Control

init?(coder: NSCoder)

Initializes a control with data in an unarchiver.

