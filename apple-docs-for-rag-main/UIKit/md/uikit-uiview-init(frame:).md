

- UIKit
- UIView
-  init(frame:) 

Initializer

# init(frame:)

Creates a view with the specified frame rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(frame: CGRect)
```

## Parameters 

`frame`  

The frame rectangle for the view, measured in points. The origin of the frame is relative to the superview in which you plan to add it. This method uses the frame rectangle to set the center and bounds properties accordingly.

## Return Value

An initialized view object.

## Discussion

The new view object must be inserted into the view hierarchy of a window before it can be used. If you create a view object programmatically, this method is the designated initializer for the UIView class. Subclasses can override this method to perform any custom initialization but must call `super` at the beginning of their implementation.

If you use Interface Builder to design your interface, this method is not called when your view objects are subsequently loaded from the nib file. Objects in a nib file are reconstituted and then initialized using their init(coder:) method, which modifies the attributes of the view to match the attributes stored in the nib file. For detailed information about how views are loaded from a nib file, see Resource Programming Guide.

## See Also

### Creating a view object

init?(coder: NSCoder)

Creates a view from data in an unarchiver.

