

- User Notifications
- UNNotificationAttachment
-  url 

Instance Property

# url

The URL of the file for this attachment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var url: URL { get }
```

## Discussion

The file at the specified URL is security scoped to your app. Before you access it, call the startAccessingSecurityScopedResource() method of NSURL.

## See Also

### Getting the Attachment Contents

var identifier: String

The unique identifier for the attachment.

var type: String

The UTI type of the attachment.

