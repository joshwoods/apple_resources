

- Quick Look UI
- QLPreviewPanel
-  enterFullScreenMode(\_:withOptions:) 

Instance Method

# enterFullScreenMode(\_:withOptions:)

Instructs the panel to enter full screen mode.

macOS 10.6+

``` source
@MainActor
func enterFullScreenMode(
    _ screen: NSScreen!,
    withOptions options: [AnyHashable : Any]! = [:]
) -> Bool
```

## Parameters 

`screen`  

This parameter isn’t currently used—pass `nil`.

`options`  

This parameter isn’t currently used—pass `nil`.

## Return Value

true if the panel was able to enter full screen mode; otherwise, false.

## Discussion

If the panel isn’t onscreen, the panel goes directly to full screen mode.

The panel chooses the appropriate screen depending on where the panel is or, if entering fullscreen directly, where the panel zooms from.

## See Also

### Managing Full Screen Mode

func exitFullScreenMode(options: [AnyHashable : Any]!)

Instructs the panel to exit full screen mode.

var isInFullScreenMode: Bool

The property that indicates whether the panel is in full screen mode.

