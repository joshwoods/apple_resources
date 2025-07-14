

- Screen Saver
- ScreenSaverView
-  hasConfigureSheet 

Instance Property

# hasConfigureSheet

A Boolean value that indicates whether the screen saver has an associated configuration sheet.

macOS 10.0+

``` source
@MainActor
var hasConfigureSheet: Bool { get }
```

## Discussion

If you provide a configuration sheet in your bundle, override this method and return true.

## See Also

### Accessing the configuration sheet

var configureSheet: NSWindow?

The window that contains the controls to configure the screen saver.

