

- AppKit
- NSViewAnimation
-  init(viewAnimations:) 

Initializer

# init(viewAnimations:)

Returns an `NSViewAnimation` object initialized with the supplied information.

macOS

``` source
init(viewAnimations: [[NSViewAnimation.Key : Any]])
```

## Parameters 

`viewAnimations`  

An array of NSDictionary objects. Each dictionary specifies a view or window to animate and the effect to apply. `viewAnimations` can be `nil`, but you must later set the required array of dictionaries with viewAnimations if you want to use the capabilities of the `NSViewAnimation` class. See`View Animation Dictionary Keys` for a description of valid keys and values for dictionaries in `viewAnimations`.

## Return Value

The created `NSViewAnimation` object or `nil` if there was a problem initializing the object.

## See Also

### Related Documentation

Cocoa Drawing Guide

