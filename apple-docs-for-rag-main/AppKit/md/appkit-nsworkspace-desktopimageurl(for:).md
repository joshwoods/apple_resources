

- AppKit
- NSWorkspace
-  desktopImageURL(for:) 

Instance Method

# desktopImageURL(for:)

Returns the URL for the desktop image for the given screen.

macOS 10.6+

``` source
func desktopImageURL(for screen: NSScreen) -> URL?
```

## Parameters 

`screen`  

The screen for which to get the desktop image.

## Return Value

The desktop image.

## Discussion

You must call this method from your app’s main thread.

## See Also

### Managing the Desktop Image

func setDesktopImageURL(URL, for: NSScreen, options: [NSWorkspace.DesktopImageOptionKey : Any]) throws

Sets the desktop image for the given screen to the image at the specified URL.

func desktopImageOptions(for: NSScreen) -> [NSWorkspace.DesktopImageOptionKey : Any]?

Returns the desktop image options for the given screen.

struct DesktopImageOptionKey

Keys that indicate how to display a new desktop image.

