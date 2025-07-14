

- Quick Look UI
- QLPreviewPanel
-  isInFullScreenMode 

Instance Property

# isInFullScreenMode

The property that indicates whether the panel is in full screen mode.

macOS 10.6+

``` source
@MainActor
var isInFullScreenMode: Bool { get }
```

## Discussion

The value is true if the panel is currently open and in full screen mode; otherwise it’s false.

## See Also

### Managing Full Screen Mode

func enterFullScreenMode(NSScreen!, withOptions: [AnyHashable : Any]!) -> Bool

Instructs the panel to enter full screen mode.

func exitFullScreenMode(options: [AnyHashable : Any]!)

Instructs the panel to exit full screen mode.

