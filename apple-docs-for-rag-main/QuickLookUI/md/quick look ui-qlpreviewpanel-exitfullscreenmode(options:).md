

- Quick Look UI
- QLPreviewPanel
-  exitFullScreenMode(options:) 

Instance Method

# exitFullScreenMode(options:)

Instructs the panel to exit full screen mode.

macOS 10.6+

``` source
@MainActor
func exitFullScreenMode(options: [AnyHashable : Any]! = [:])
```

## Parameters 

`options`  

This parameter isn’t used — pass `nil`.

## See Also

### Managing Full Screen Mode

func enterFullScreenMode(NSScreen!, withOptions: [AnyHashable : Any]!) -> Bool

Instructs the panel to enter full screen mode.

var isInFullScreenMode: Bool

The property that indicates whether the panel is in full screen mode.

