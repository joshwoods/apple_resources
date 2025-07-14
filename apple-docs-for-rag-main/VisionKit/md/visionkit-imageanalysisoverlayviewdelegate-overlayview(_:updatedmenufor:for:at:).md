

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:updatedMenuFor:for:at:) 

Instance Method

# overlayView(\_:updatedMenuFor:for:at:)

Notifies your app before the framework presents a context menu.

macOS 14.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    updatedMenuFor menu: NSMenu,
    for event: NSEvent,
    at point: CGPoint
) -> NSMenu
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The associated overlay view for the updated menu.

`menu`  

The menu that appears.

`event`  

The event associated with this menu.

`point`  

The original location of the event for the menu.

## Discussion

This callback enables your app to add custom context menu items or manage the framework-provided content menu items. For example, the following implementation changes the title of the framework-provided `copySubject` menu item from “Copy” to “Copy and remove background”.

```
func overlayView(_ overlayView: ImageAnalysisOverlayView, updateMenu menu: NSMenu, forEvent: NSEvent, atPoint point: CGPoint) -> NSMenu {

    let copySubjectItem = menu.item(withTag:ImageAnalysisOverlayView.MenuTag.copySubject)
    copySubjectItem.title = "Copy and remove background"

    return menu
}
```

The menu items don’t persist. However, your app can alter menu items and share them across different menus within the same menu session.

To add items to a menu, access the recommended index for insertion by using the recommendedAppItems menu tag, such as in the following code:

```
func overlayView(_ overlayView: ImageAnalysisOverlayView, updateMenu menu: NSMenu, forEvent: NSEvent, atPoint point: CGPoint) -> NSMenu {

    let item = NSMenuItem()
    let tag = ImageAnalysisOverlayView.MenuTag.recommendedAppItems
    let index = menu.indexOfItem(withTag:tag)
    menu.insertItem(item, at: index)

    return menu
}
```

Note

The framework is the delegate for the returned menu item. The framework continues to support NSMenuDelegate callbacks for VisionKit-specific menu items.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, updatedMenuFor: NSMenu, for: NSEvent, at: CGPoint) -> NSMenu

A default implementation that returns the menu without any changes.

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

func overlayView(ImageAnalysisOverlayView, didClose: NSMenu)

Notifies your app that the given menu closed.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, needsUpdate: NSMenu)

Notifies your app that the given menu needs updating.

**Required** Default implementation provided.

