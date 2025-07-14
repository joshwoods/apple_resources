

- PDFKit
- PDFDocumentDelegate
-  documentDidFindMatch(\_:) 

Instance Method

# documentDidFindMatch(\_:)

Called when the `PDFDocumentDidFindMatchNotification` notification is posted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func documentDidFindMatch(_ notification: Notification)
```

## See Also

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

