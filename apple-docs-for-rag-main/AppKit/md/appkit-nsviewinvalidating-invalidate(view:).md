

- AppKit
- NSViewInvalidating
-  invalidate(view:) 

Instance Method

# invalidate(view:)

Indicates to the system that an aspect of a view is invalid and triggers the necessary update.

macOS 12.0+Swift 5.1+

``` source
func invalidate(view: NSView)
```

**Required**

## Parameters 

`view`  

The view that requires invalidating.

## Discussion

A type that conforms to `UIViewInvalidating` implements this method to perform any actions necessary to notify the system that an aspect of your view is invalid. For more info, see NSView.Invalidating.

## See Also

### Supporting Types

enum Invalidations

Changes that cause aspects of a view to be invalid and require an update.

