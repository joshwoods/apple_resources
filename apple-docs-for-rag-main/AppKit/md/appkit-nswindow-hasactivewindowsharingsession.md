

- AppKit
- NSWindow
-  hasActiveWindowSharingSession 

Instance Property

# hasActiveWindowSharingSession

macOS 13.3+

``` source
@MainActor
var hasActiveWindowSharingSession: Bool { get }
```

## See Also

### Managing Window Sharing

func transferWindowSharing(to: NSWindow, completionHandler: ((any Error)?) -> Void)

