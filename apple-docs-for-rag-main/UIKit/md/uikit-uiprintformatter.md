

- UIKit
-  UIPrintFormatter 

Class

# UIPrintFormatter

An abstract base class for print formatters, which are objects that lay out custom printable content that can cross page boundaries.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPrintFormatter
```

## Overview

Given a print formatter, the printing system can automate the printing of the type of content associated with the print formatter. Examples of such content could be a web view, a mix of images and text, or a long text document. The UIKit framework provides several concrete subclasses of UIPrintFormatter: UISimpleTextPrintFormatter, UIMarkupTextPrintFormatter, and UIViewPrintFormatter.

You can assign a single print formatter for a print job using the printFormatter property of the UIPrintInteractionController shared instance; or you can specify one or more print formatters that are associated with specific pages of a page renderer through the addPrintFormatter(_:startingAtPageAt:)method of UIPrintPageRenderer. A page renderer is an instance of a custom subclass of UIPrintPageRenderer that draws content for printing.

UIPrintFormatter publishes an interface that allows you to specify the starting page for a print job and the margins around the printed content; given that information plus the content, a print formatter computes the number of pages for the print job. The following image depicts the print-formatter properties, along with certain UIPrintPaper and UIPrintPageRenderer properties, that define the layout of a multipage print job.

Third-party subclasses of UIPrintFormatter aren’t recommended. If you have custom content to print, use a custom UIPrintPageRenderer object.

## Topics

### Laying out the content

var perPageContentInsets: UIEdgeInsets

The margins for each printed page.

var maximumContentHeight: CGFloat

The maximum height of the content area.

var maximumContentWidth: CGFloat

The maximum width of the content area.

var contentInsets: UIEdgeInsets

The distances the edges of content are inset from the printing rectangle.

Deprecated

### Managing pagination

var startPage: Int

The index of the first page that the print formatter lays out.

var pageCount: Int

The number of pages to print.

### Drawing the content

func draw(in: CGRect, forPageAt: Int)

Draws the portion of a print formatter’s content for the specified area of the specified page.

func rectForPage(at: Int) -> CGRect

Returns the area that encloses a specified page of content.

### Communicating with the page renderer

func removeFromPrintPageRenderer()

Removes the print formatter from the page renderer.

var printPageRenderer: UIPrintPageRenderer?

Returns the page renderer for the print formatter.

### Requiring operations to take place on the main thread

var requiresMainThread: Bool

A Boolean value that determines whether the system executes the print formatter’s rendering operations on the main thread.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIMarkupTextPrintFormatter
- UISimpleTextPrintFormatter
- UIViewPrintFormatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Formatters

class UIViewPrintFormatter

An object that lays out the drawn content of a view for printing.

class UISimpleTextPrintFormatter

An object that lays out plain text for printing, possibly over multiple pages.

class UIMarkupTextPrintFormatter

An object that lays out HTML text for a multipage print job.

