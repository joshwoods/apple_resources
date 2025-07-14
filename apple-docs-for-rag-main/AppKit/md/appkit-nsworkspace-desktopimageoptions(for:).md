

- AppKit
- NSWorkspace
-  desktopImageOptions(for:) 

Instance Method

# desktopImageOptions(for:)

Returns the desktop image options for the given screen.

macOS 10.6+

``` source
func desktopImageOptions(for screen: NSScreen) -> [NSWorkspace.DesktopImageOptionKey : Any]?
```

## Parameters 

`screen`  

The screen for which to get the desktop image options.

## Return Value

A dictionary containing the keys found in NSWorkspace.DesktopImageOptionKey.

## Discussion

You must call this method from your app’s main thread.

## See Also

### Managing the Desktop Image

func desktopImageURL(for: NSScreen) -> URL?

Returns the URL for the desktop image for the given screen.

func setDesktopImageURL(URL, for: NSScreen, options: [NSWorkspace.DesktopImageOptionKey : Any]) throws

Sets the desktop image for the given screen to the image at the specified URL.

struct DesktopImageOptionKey

Keys that indicate how to display a new desktop image.

