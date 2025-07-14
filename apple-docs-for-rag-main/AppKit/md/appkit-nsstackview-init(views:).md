

- AppKit
- NSStackView
-  init(views:) 

Initializer

# init(views:)

Creates and returns a stack view with a specified array of views.

macOS 10.9+

``` source
@MainActor
convenience init(views: [NSView])
```

## Parameters 

`views`  

The array of views for the new stack view.

## Return Value

A stack view initialized with the specified array of views.

## Discussion

The returned stack view has horizontal layout direction and its translatesAutoresizingMaskIntoConstraints property is set to the Boolean value false. The views you provide in the `views` parameter are placed into the stack view’s leading gravity area.

## See Also

### Related Documentation

View Programming Guide

Auto Layout Guide

