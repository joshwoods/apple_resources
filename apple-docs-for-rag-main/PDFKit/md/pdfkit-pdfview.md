

- PDFKit
-  PDFView 

Class

# PDFView

An object that encapsulates the functionality of PDF Kit into a single widget that you can add to your application using Interface Builder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class PDFView
```

## Mentioned in 

Adding Custom Graphics to a PDF

## Overview

`PDFView` may be the only class you need to deal with for adding PDF functionality to your application. It lets you display PDF data and allows users to select content, navigate through a document, set zoom level, and copy textual content to the Pasteboard. `PDFView` also keeps track of page history.

You can subclass `PDFView` to create a custom PDF viewer.

You can also create a custom PDF viewer by using the PDF Kit utility classes directly and not using `PDFView` at all.

## Topics

### Associating a Document with a View

var document: PDFDocument?

Returns the document associated with a `PDFView` object.

func takePasswordFrom(Any)

Unlocks with the password from the specified sender.

Deprecated

### Configuring Document View

Configurations

Define display modes, scaling, rendering, printing and graphics properties.

### Interacting in a View

Document Interactions

Handle selections, work with annotation actions, convert page and view points, and work with mouse events in a document.

### Navigating Within a Document

var currentPage: PDFPage?

Returns the current page.

var currentDestination: PDFDestination?

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

var visiblePages: [PDFPage]

Returns an array of `PDFPage` objects that represent the currently visible pages.

Navigation

Operations for moving through page history and seeking to a page in a document.

### Setting the Delegate

var delegate: (any PDFViewDelegate)?

Returns the view’s delegate.

protocol PDFViewDelegate

The delegate for the `PDFView` object.

### Instance Properties

var findInteraction: UIFindInteraction

var isFindInteractionEnabled: Bool

var isInMarkupMode: Bool

var pageOverlayViewProvider: (any PDFPageOverlayViewProvider)?

var pageShadowsEnabled: Bool

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
- NSAnimationDelegate
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSMenuDelegate
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFindInteractionDelegate
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIGestureRecognizerDelegate
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views

class PDFThumbnailView

An object that contains a set of thumbnails, each of which represents a page in a PDF document.

