

- Quick Look UI
- QLPreviewReply
-  attachments 

Instance Property

# attachments

The attachments for a preview reply that provide additional data for the system to display the preview.

macOS 12.0+

``` source
var attachments: [String : QLPreviewReplyAttachment] { get set }
```

## Discussion

When providing an HTML reply, use the string associated with the QLPreviewReplyAttachment prefixed with `cid:` to reference the content within the HTML.

## See Also

### Inspecting a preview reply

var title: String

The title for the system to display with the preview.

var stringEncoding: String.Encoding

