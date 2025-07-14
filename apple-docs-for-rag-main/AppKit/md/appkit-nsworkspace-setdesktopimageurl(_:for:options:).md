

- AppKit
- NSWorkspace
-  setDesktopImageURL(\_:for:options:) 

Instance Method

# setDesktopImageURL(\_:for:options:)

Sets the desktop image for the given screen to the image at the specified URL.

macOS 10.6+

``` source
func setDesktopImageURL(
    _ url: URL,
    for screen: NSScreen,
    options: [NSWorkspace.DesktopImageOptionKey : Any] = [:]
) throws
```

## Parameters 

`url`  

A file URL to the image. The URL must not be `nil`.

`screen`  

The screen on which to set the desktop image.

`options`  

The options dictionary may contain any of the keys in NSWorkspace.DesktopImageOptionKey, which control how the image is scaled on the screen.

## Discussion

Instead of presenting a user interface for picking the options, choose appropriate defaults and allow the user to adjust them in the System Preference Pane.

You must call this method from your app’s main thread.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing the Desktop Image

func desktopImageURL(for: NSScreen) -> URL?

Returns the URL for the desktop image for the given screen.

func desktopImageOptions(for: NSScreen) -> [NSWorkspace.DesktopImageOptionKey : Any]?

Returns the desktop image options for the given screen.

struct DesktopImageOptionKey

Keys that indicate how to display a new desktop image.

