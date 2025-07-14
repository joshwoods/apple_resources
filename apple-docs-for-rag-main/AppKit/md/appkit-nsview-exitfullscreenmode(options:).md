

- AppKit
- NSView
-  exitFullScreenMode(options:) 

Instance Method

# exitFullScreenMode(options:)

Instructs the view to exit full screen mode.

macOS 10.5+

``` source
@MainActor
func exitFullScreenMode(options: [NSView.FullScreenModeOptionKey : Any]? = nil)
```

## Parameters 

`options`  

A dictionary of options for the mode. For possible keys, see `Full Screen Mode Options`.

## Discussion

When the fullScreenModeApplicationPresentationOptions options is specified when enterFullScreenMode(_:withOptions:) is invoked, exiting full screen mode will restore the previously active presentationOptions.

## See Also

### Drawing the View in Fullscreen Mode

func enterFullScreenMode(NSScreen, withOptions: [NSView.FullScreenModeOptionKey : Any]?) -> Bool

Sets the view to full screen mode.

var isInFullScreenMode: Bool

A Boolean value indicating whether the view is in full screen mode.

struct FullScreenModeOptionKey

These constants are keys that you can use in the options dictionary in enterFullScreenMode(_:withOptions:) and exitFullScreenMode(options:).

