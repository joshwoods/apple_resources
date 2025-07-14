

- VisionKit
- ImageAnalysisOverlayView
-  ImageAnalysisOverlayView.MenuTag 

Structure

# ImageAnalysisOverlayView.MenuTag

Tags that enable your app to manage image-analysis context menu items.

macOS 14.0+

``` source
struct MenuTag
```

## Overview

Manage app context menu items by implementing the ImageAnalysisOverlayViewDelegate menu-related callbacks and referencing the menu item instances using tags from this enumeration. For example, see overlayView(_:updatedMenuFor:for:at:).

## Topics

### Manage Framework-provided menu items

static let copyImage: Int

An index for the copy-image menu item.

static let shareImage: Int

An index for the share-image menu item.

static let copySubject: Int

An index for the copy-subject menu item.

static let shareSubject: Int

An index for the share-subject menu item.

static let lookupItem: Int

An index for the Visual Look Up menu item.

### Create app-defined menu items

static let recommendedAppItems: Int

An index for app-provided menu items.

## See Also

### Customizing the interface

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Text button and the interface for Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: NSEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: NSFont?

The font to use for the supplementary interface.

