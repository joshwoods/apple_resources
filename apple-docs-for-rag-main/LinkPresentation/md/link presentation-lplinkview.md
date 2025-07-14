

- Link Presentation
-  LPLinkView 

Class

# LPLinkView

A rich visual representation of a link.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class LPLinkView
```

## Overview

LPLinkView presents a link based on its available metadata. Use it to show a link’s title and icon, associated images, inline audio, video playback, and maps in a familiar and consistent style.

## Present a rich link

To present a rich link in your app, create an LPLinkView, passing an LPLinkMetadata instance into its initializer. Then add the LPLinkView to your view.

For example, to present links in a table view, add an LPLinkView instance as a subview when populating each cell.

```
let linkView = LPLinkView(metadata: metadata)
cell.contentView.addSubview(linkView)
linkView.sizeToFit()
```

LPLinkView has an intrinsic size, but it also responds to sizeToFit() to present a layout at any size.

## Topics

### Creating a link view

init(metadata: LPLinkMetadata)

Initializes a link view with specified metadata.

init(url: URL)

Initializes a placeholder link view without metadata for a given URL.

### Specifying metadata

var metadata: LPLinkMetadata

The metadata from which to generate a rich presentation.

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

