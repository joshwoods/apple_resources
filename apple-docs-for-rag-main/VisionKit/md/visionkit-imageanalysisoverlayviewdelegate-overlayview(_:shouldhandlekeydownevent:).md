

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:shouldHandleKeyDownEvent:) 

Instance Method

# overlayView(\_:shouldHandleKeyDownEvent:)

Returns a Boolean value that indicates whether the overlay view consumes the given key-down event.

macOS 13.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    shouldHandleKeyDownEvent event: NSEvent
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The overlay view that receives the key-down event.

`event`  

The key-down event that occurs.

## Return Value

`true` if the overlay view handles the event; otherwise, `false`.

## Discussion

The default return value is `true`. Implement this callback if you don’t want the overlay view to consume the given event.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, shouldHandleKeyDownEvent: NSEvent) -> Bool

A default implementation that indicates the overlay view handles the given key-down event.

## See Also

### Responding to key and menu events

func overlayView(ImageAnalysisOverlayView, shouldShowMenuForEvent: NSEvent, atPoint: CGPoint) -> Bool

Provides a Boolean value that indicates whether the overlay view shows a menu for the given event.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, menu: NSMenu, willHighlight: NSMenuItem?)

Notifies your app that the given menu item is highlighted.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, willOpen: NSMenu)

Notifies your app that a given menu is opening imminently.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, didClose: NSMenu)

Notifies your app that the given menu closed.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, needsUpdate: NSMenu)

Notifies your app that the given menu needs updating.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, updatedMenuFor: NSMenu, for: NSEvent, at: CGPoint) -> NSMenu

Notifies your app before the framework presents a context menu.

**Required** Default implementation provided.

