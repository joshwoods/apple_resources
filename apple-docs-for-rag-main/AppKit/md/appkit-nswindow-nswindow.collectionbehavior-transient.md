

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  transient 

Type Property

# transient

The window floats in Spaces and hides in Mission Control.

macOS 10.6+

``` source
static var transient: NSWindow.CollectionBehavior { get }
```

## Discussion

This is the default behavior if `windowLevel` isn’t equal to normal.

## See Also

### Spaces and Mission Control

static var managed: NSWindow.CollectionBehavior

The window participates in Mission Control and Spaces.

