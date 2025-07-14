

- AppKit
- NSWindow
-  transferWindowSharing(to:completionHandler:) 

Instance Method

# transferWindowSharing(to:completionHandler:)

macOS 13.3+

``` source
@MainActor
func transferWindowSharing(
    to window: NSWindow,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
func transferWindowSharing(to window: NSWindow) async throws
```

## Discussion

## See Also

### Managing Window Sharing

var hasActiveWindowSharingSession: Bool

