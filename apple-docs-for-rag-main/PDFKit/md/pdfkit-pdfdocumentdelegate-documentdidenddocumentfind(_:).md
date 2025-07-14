

- PDFKit
- PDFDocumentDelegate
-  documentDidEndDocumentFind(\_:) 

Instance Method

# documentDidEndDocumentFind(\_:)

Called when the `PDFDocumentDidEndFindNotification` notification is posted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func documentDidEndDocumentFind(_ notification: Notification)
```

## See Also

### Getting Document Search Notifications

func didMatchString(PDFSelection)

Called for every match found during a find operation.

func documentDidBeginDocumentFind(Notification)

Called when the `PDFDocumentDidBeginFindNotification` notification is posted.

func documentDidBeginPageFind(Notification)

Called when the `PDFDocumentDidBeginPageFindNotification` notification is posted.

func documentDidEndPageFind(Notification)

Called when the `PDFDocumentDidEndPageFindNotification` notification is posted.

func documentDidFindMatch(Notification)

Called when the `PDFDocumentDidFindMatchNotification` notification is posted.

