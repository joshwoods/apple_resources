

- Foundation
- NSNotification
- NSNotification.Name
-  PDFViewDisplayBoxChanged 

Type Property

# PDFViewDisplayBoxChanged

A notification posted when the display box has changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
static let PDFViewDisplayBoxChanged: NSNotification.Name
```

## Discussion

The notification object is the `PDFView` object itself.

## See Also

### PDFKit

static let PDFDocumentDidBeginFind: NSNotification.Name

A notification that the beginFindString(_:withOptions:) or findString(_:withOptions:) method begins finding.

static let PDFDocumentDidBeginPageFind: NSNotification.Name

A notification that a find operation begins working on a new page of a document.

static let PDFDocumentDidBeginPageWrite: NSNotification.Name

A notification that a write operation begins working on a page in a document.

static let PDFDocumentDidBeginWrite: NSNotification.Name

A notification that a write operation begins working on a document.

static let PDFDocumentDidEndFind: NSNotification.Name

A notification that the beginFindString(_:withOptions:) or findString(_:withOptions:) method returns.

static let PDFDocumentDidEndPageFind: NSNotification.Name

A notification that a find operation finishes working on a page in a document.

static let PDFDocumentDidEndPageWrite: NSNotification.Name

A notification that a write operation finishes working on a page in a document.

static let PDFDocumentDidEndWrite: NSNotification.Name

A notification that a write operation finishes working on a document.

static let PDFDocumentDidFindMatch: NSNotification.Name

A notification that a string match is found in a document.

static let PDFDocumentDidUnlock: NSNotification.Name

A notification that a document unlocks after a unlock(withPassword:) message.

static let PDFThumbnailViewDocumentEdited: NSNotification.Name

static let PDFViewAnnotationHit: NSNotification.Name

A notification posted when the user clicks on an annotation.

static let PDFViewAnnotationWillHit: NSNotification.Name

A notification posted before the user clicks an annotation.

static let PDFViewChangedHistory: NSNotification.Name

A notification posted when the page history changes.

static let PDFViewCopyPermission: NSNotification.Name

A notification posted when the user attempts to copy to the pasteboard without the appropriate permissions.

