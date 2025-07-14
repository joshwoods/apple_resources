

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:didClose:) 

Instance Method

# overlayView(\_:didClose:)

Notifies your app that the given menu closed.

macOS 14.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    didClose menu: NSMenu
)
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The associated overlay view for the menu.

`menu`  

The menu that closed.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, didClose: NSMenu)

A default, blank implementation for when an overlay view menu closes.

## See Also

### Responding to key and menu events

func overlayView(ImageAnalysisOverlayView, shouldHandleKeyDownEvent: NSEvent) -> Bool

Returns a Boolean value that indicates whether the overlay view consumes the given key-down event.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, shouldShowMenuForEvent: NSEvent, atPoint: CGPoint) -> Bool

Provides a Boolean value that indicates whether the overlay view shows a menu for the given event.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, menu: NSMenu, willHighlight: NSMenuItem?)

Notifies your app that the given menu item is highlighted.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, willOpen: NSMenu)

Notifies your app that a given menu is opening imminently.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, needsUpdate: NSMenu)

Notifies your app that the given menu needs updating.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, updatedMenuFor: NSMenu, for: NSEvent, at: CGPoint) -> NSMenu

Notifies your app before the framework presents a context menu.

**Required** Default implementation provided.

