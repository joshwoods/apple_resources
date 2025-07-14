

- PDFKit
- PDFDocumentDelegate
-  didMatchString(\_:) 

Instance Method

# didMatchString(\_:)

Called for every match found during a find operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
optional func didMatchString(_ instance: PDFSelection)
```

## See Also

### Getting Document Search Notifications

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

