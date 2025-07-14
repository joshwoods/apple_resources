

- PDFKit
-  PDFDocumentDelegate 

Protocol

# PDFDocumentDelegate

The delegate for the `PDFDocument` object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
protocol PDFDocumentDelegate : NSObjectProtocol
```

## Mentioned in 

Adding Custom Graphics to a PDF

## Topics

### Managing Document Security

func documentDidUnlock(Notification)

Called when the `PDFDocumentDidUnlockNotification` notification is posted.

### Getting Document Search Notifications

func didMatchString(PDFSelection)

Called for every match found during a find operation.

func documentDidBeginDocumentFind(Notification)

Called when the `PDFDocumentDidBeginFindNotification` notification is posted.

func documentDidBeginPageFind(Notification)

Called when the `PDFDocumentDidBeginPageFindNotification` notification is posted.

func documentDidEndDocumentFind(Notification)

Called when the `PDFDocumentDidEndFindNotification` notification is posted.

func documentDidEndPageFind(Notification)

Called when the `PDFDocumentDidEndPageFindNotification` notification is posted.

func documentDidFindMatch(Notification)

Called when the `PDFDocumentDidFindMatchNotification` notification is posted.

### Wrapping Document Elements

func classForPage() -> AnyClass

Returns a `PDFPage` subclass for a page object.

func `class`(forAnnotationClass: AnyClass) -> AnyClass

Returns a `PDFAnnotation` subclass for a class.

Deprecated

func `class`(forAnnotationType: String) -> AnyClass

Returns a `PDFAnnotation` subclass for an annotation type.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the Delegate

var delegate: (any PDFDocumentDelegate)?

The object acting as the delegate for the `PDFDocument` object.

