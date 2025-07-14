

- UIKit
-  Printing 

API Collection

# Printing

Display the system print panels and manage the printing process.

## Topics

### Print panels

class UIPrintInteractionController

A user interface that manages the printing of documents, images, and other printable content in iOS.

class UIPrinterPickerController

A view controller that displays the standard interface for selecting a printer.

### Renderer

class UIPrintPageRenderer

An object that draws pages of content to print, with or without the assistance of print formatters.

Building and improving your app with Mac Catalyst

Improve your iPadOS app with Mac Catalyst by supporting native controls, multiple windows, sharing, printing, menus and keyboard shortcuts.

### Job info

class UIPrinter

A printer on the network.

class UIPrintInfo

Information about a print job that the system uses when it prints.

class UIPrintPaper

The size of paper for a print job and the rectangular area that the content prints within.

### Formatters

class UIPrintFormatter

An abstract base class for print formatters, which are objects that lay out custom printable content that can cross page boundaries.

class UIViewPrintFormatter

An object that lays out the drawn content of a view for printing.

class UISimpleTextPrintFormatter

An object that lays out plain text for printing, possibly over multiple pages.

class UIMarkupTextPrintFormatter

An object that lays out HTML text for a multipage print job.

### Printer service discovery

class UIPrintServiceExtension

An extension that locates and sets up a printer without a configuration profile.

class UIPrinterDestination

A description of a single printer.

### Keyboard shortcut

UIApplicationSupportsPrintCommand

A Boolean value that indicates whether the app supports the Command-P keyboard shortcut.

## See Also

### Graphics, drawing, and printing

Images and PDF

Create and manage images, including those that use bitmap and PDF formats.

Drawing

Configure your app’s drawing environment using colors, renderers, draw paths, strings, and shadows.

