

- AppKit
- NSView
-  enterFullScreenMode(\_:withOptions:) 

Instance Method

# enterFullScreenMode(\_:withOptions:)

Sets the view to full screen mode.

macOS 10.5+

``` source
@MainActor
func enterFullScreenMode(
    _ screen: NSScreen,
    withOptions options: [NSView.FullScreenModeOptionKey : Any]? = nil
) -> Bool
```

## Parameters 

`screen`  

The screen the view should cover.

`options`  

A dictionary of options for the mode. For possible keys, see `Full Screen Mode Options`.

## Return Value

true if the view was able to enter full screen mode, otherwise false.

## Discussion

When the fullScreenModeApplicationPresentationOptions is contained in the options dictionary, the presentation options that were in effect when this method is invoked are not altered, and no displays are captured.

If you do not wish to capture the screen when going to full screen mode, you can add fullScreenModeApplicationPresentationOptions to the options dictionary with the value returned by the presentationOptions.

When the fullScreenModeApplicationPresentationOptions options is specified, exiting full screen mode using exitFullScreenMode(options:) will restore the previously active presentationOptions.

### Special Considerations

In OS X v 10.5, invoking this method when the view was not in a window would cause an exception. In macOS 10.6 and later, you can now send this message to a view not in a window. For applications that must also run in OS X v 10.5, a simple workaround is to place the view in an offscreen window.

## See Also

### Drawing the View in Fullscreen Mode

func exitFullScreenMode(options: [NSView.FullScreenModeOptionKey : Any]?)

Instructs the view to exit full screen mode.

var isInFullScreenMode: Bool

A Boolean value indicating whether the view is in full screen mode.

struct FullScreenModeOptionKey

These constants are keys that you can use in the options dictionary in enterFullScreenMode(_:withOptions:) and exitFullScreenMode(options:).

