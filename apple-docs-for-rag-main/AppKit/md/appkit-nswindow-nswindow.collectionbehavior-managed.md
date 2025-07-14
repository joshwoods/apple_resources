

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  managed 

Type Property

# managed

The window participates in Mission Control and Spaces.

macOS 10.6+

``` source
static var managed: NSWindow.CollectionBehavior { get }
```

## Discussion

This is the default behavior if `windowLevel` is equal to normal.

## See Also

### Spaces and Mission Control

static var transient: NSWindow.CollectionBehavior

The window floats in Spaces and hides in Mission Control.

