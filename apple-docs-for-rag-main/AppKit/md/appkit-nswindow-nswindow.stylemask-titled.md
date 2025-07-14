

- AppKit
- NSWindow
- NSWindow.StyleMask
-  titled 

Type Property

# titled

The window displays a title bar.

macOS

``` source
static var titled: NSWindow.StyleMask { get }
```

## See Also

### Constants

static var borderless: NSWindow.StyleMask

The window displays none of the usual peripheral elements. Useful only for display or caching purposes. A window that uses `NSWindowStyleMaskBorderless` can’t become key or main, unless the value of canBecomeKey or canBecomeMain is true. Note that you can set a window’s or panel’s style mask to `NSWindowStyleMaskBorderless` in Interface Builder by deselecting Title Bar in the Appearance section of the Attributes inspector.

static var closable: NSWindow.StyleMask

The window displays a close button.

static var miniaturizable: NSWindow.StyleMask

The window displays a minimize button.

static var resizable: NSWindow.StyleMask

The window can be resized by the user.

static var texturedBackground: NSWindow.StyleMask

The window uses a textured background that darkens when the window is key or main and lightens when it is inactive, and may have a second gradient in the section below the window content.

Deprecated

static var unifiedTitleAndToolbar: NSWindow.StyleMask

This constant has no effect, because all windows that include a toolbar use the unified style.

static var fullScreen: NSWindow.StyleMask

The window can appear full screen. A fullscreen window does not draw its title bar, and may have special handling for its toolbar. (This mask is automatically toggled when toggleFullScreen(_:) is called.)

static var fullSizeContentView: NSWindow.StyleMask

When set, the window’s contentView consumes the full size of the window. Although you can combine this constant with other window style masks, it is respected only for windows with a title bar. Note that using this mask opts in to layer-backing. Use the contentLayoutRect or the contentLayoutGuide to lay out views underneath the title bar–toolbar area.

static var utilityWindow: NSWindow.StyleMask

The window is a panel or a subclass of NSPanel.

static var docModalWindow: NSWindow.StyleMask

The window is a document-modal panel (or a subclass of NSPanel).

static var nonactivatingPanel: NSWindow.StyleMask

The window is a panel or a subclass of NSPanel that does not activate the owning app.

static var hudWindow: NSWindow.StyleMask

The window is a HUD panel.

