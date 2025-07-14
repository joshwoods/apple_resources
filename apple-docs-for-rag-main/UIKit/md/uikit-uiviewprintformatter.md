

- UIKit
-  UIViewPrintFormatter 

Class

# UIViewPrintFormatter

An object that lays out the drawn content of a view for printing.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIViewPrintFormatter
```

## Overview

Instances of three system classes offer usable view print formatters to applications: UIWebView and UITextView of the UIKit framework, and MKMapView of the MapKit framework. To obtain a view print formatter for a print job, call the UIView method viewPrintFormatter() and initialize the print formatter’s inherited layout properties.

Add the print formatter to the print job in one of two ways:

- If a single print formatter is being used for the print job (with no additional drawing), assign it to the printFormatter property of the UIPrintInteractionController shared instance. The inherited startPage property identifies the beginning page of content with which the formatter is associated.

- If you are using multiple formatters along with a page renderer, associate each print formatter with a starting page of the printed content. You often take this approach when you want to add content such as headers and footers to what the formatters provide. You have two ways of associating a print formatter with a UIPrintPageRenderer object:

- You can add print formatters to the printFormatters property of the UIPrintPageRenderer object; the startPage property of the print formatter specifies the starting page

- You can add print formatters by calling addPrintFormatter(_:startingAtPageAt:) for each print formatter; the second parameter of this method specifies the starting page (and overrides any startPage value).

View print formatters typically implement the UIView method draw(_:for:) to draw content in a way that is suitable for printing, If they don’t implement this method, their draw(_:) method is called instead.

### Subclassing Notes

Subclassing `UIViewPrintFormatter` to print the contents of a view is not recommended. To print the contents of a custom view, you should instead draw the view’s contents for printing using a custom UIPrintPageRenderer object.

## Topics

### Accessing the view

var view: UIView

The view from which the view print formatter was derived.

## Relationships

### Inherits From

- UIPrintFormatter

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

class UIPrintFormatter

An abstract base class for print formatters, which are objects that lay out custom printable content that can cross page boundaries.

class UISimpleTextPrintFormatter

An object that lays out plain text for printing, possibly over multiple pages.

class UIMarkupTextPrintFormatter

An object that lays out HTML text for a multipage print job.

