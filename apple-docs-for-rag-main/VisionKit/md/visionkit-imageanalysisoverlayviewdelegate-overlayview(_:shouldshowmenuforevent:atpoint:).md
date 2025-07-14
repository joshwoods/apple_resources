

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:shouldShowMenuForEvent:atPoint:) 

Instance Method

# overlayView(\_:shouldShowMenuForEvent:atPoint:)

Provides a Boolean value that indicates whether the overlay view shows a menu for the given event.

macOS 13.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    shouldShowMenuForEvent event: NSEvent,
    atPoint point: CGPoint
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The overlay view in which the menu appears.

`event`  

The event that occurs.

`point`  

The location of the event.

## Return Value

`true` if the menu appears in the overlay; otherwise, `false`.

## Discussion

Implement this method if you don’t want the overlay view to show a menu for a specific event at a location. The default return value is `true`.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, shouldShowMenuForEvent: NSEvent, atPoint: CGPoint) -> Bool

A default implementation that indicates the overlay view shows its menu for the given event.

## See Also

### Responding to key and menu events

func overlayView(ImageAnalysisOverlayView, shouldHandleKeyDownEvent: NSEvent) -> Bool

Returns a Boolean value that indicates whether the overlay view consumes the given key-down event.

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

