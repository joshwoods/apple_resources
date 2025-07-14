

- UIKit
-  UIDocumentProperties 

Class

# UIDocumentProperties

Information that UIKit uses to generate a document header for a navigation item’s title menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UIDocumentProperties
```

## Overview

Assign a UIDocumentProperties object to your navigation item’s documentProperties property. UIKit uses this object to display a document header at the top of the title menu, which appears when a person taps the navigation item’s title. The document header displays information about the current document, such as its title, file type, and size.

Additionally, you can configure a set of sharing capabilities that allow people to share or drag and drop the document content from the document header:

- Set an activityViewControllerProvider to show the Share button.

- Set a dragItemsProvider to allow people to drag and drop the document by dragging the preview icon.

Related Sessions from WWDC22

Session 10069: Meet desktop-class iPad

Session 10070: Build a desktop-class iPad app

## Topics

### Creating a document header

init(url: URL)

Creates a document properties object from document data at the URL you specify.

init(metadata: LPLinkMetadata)

Creates a document properties object from the metadata object you specify.

var metadata: LPLinkMetadata

The document’s metadata.

### Generating a document preview

var wantsIconRepresentation: Bool

A Boolean value that determines whether to render an icon of the document in the navigation bar.

### Supporting drag and drop

var dragItemsProvider: ((any UIDragSession) -> [UIDragItem])?

A closure that provides drag items that represent the document.

### Supporting sharing

var activityViewControllerProvider: (() -> UIActivityViewController)?

A closure that provides an activity view controller for sharing the document.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Customizing the title menu

var titleMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that generates the navigation item’s title menu.

var documentProperties: UIDocumentProperties?

An object that provides the document header for the title menu.

