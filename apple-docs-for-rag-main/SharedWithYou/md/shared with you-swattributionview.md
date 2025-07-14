

- Shared With You
-  SWAttributionView 

Class

# SWAttributionView

A view that displays the sender who shares a highlight and provides related actions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
class SWAttributionView
```

## Mentioned in 

Making your app content shareable

## Overview

The `SWAttributionView` also allows users to get back to the conversation about the SWHighlight content, and other related actions using a highlightMenu.

Place an `SWAttributionView` next to the content represented by its `SWHighlight`. The `SWAttributionView` displays the names and avatars within the provided horizontal space.

You can constrain this view’s width anchor or set its frame width to control the maximum width of its contents after which truncation may occur. Don’t constrain the view’s height, as the height is dependent on the preferredContentSizeCategory, and the resulting font size. To provide enough vertical space around this view, reference its heightAnchor when using Auto Layout, or its intrinsicContentSize when using manual layout.

## Topics

### Customizing highlights

var backgroundStyle: SWAttributionView.BackgroundStyle

The background style of the child view that contains names and avatars.

var displayContext: SWAttributionView.DisplayContext

The context for the content the system displays with this view.

var highlight: SWHighlight?

The highlight you use to display this attribution.

var highlightMenu: UIMenu

A menu with a list of system actions specific to this hightlight.

var horizontalAlignment: SWAttributionView.HorizontalAlignment

The horizontal alignment of the view.

var menuTitleForHideAction: String?

A localized string the system uses as a custom title for the hide menu item.

var preferredMaxLayoutWidth: CGFloat

A width the system uses to constrain the view contents.

var supplementalMenu: UIMenu?

A supplemental menu to augment the attribution view’s existing menu.

### Customizing the view

enum BackgroundStyle

The background styling of the attribution view’s contents.

enum DisplayContext

The context for the content that influences the ranking of this view’s highlight.

enum HorizontalAlignment

The horizontal alignment of attribution view’s contents.

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

