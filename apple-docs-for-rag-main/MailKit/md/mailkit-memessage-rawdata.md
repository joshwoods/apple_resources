

- MailKit
- MEMessage
-  rawData 

Instance Property

# rawData

The raw RFC 2822 header and body content of the message.

macOS 12.0+

``` source
var rawData: Data? { get }
```

## Discussion

The content is available after MailKit downloads the message. MailKit provides the content as unprocessed data. For details about the format of the data, see RFC 2822.

Note

This property includes the full content of the message, and contains both the headers and the message body. If you only need the headers in the message, use headers instead.

## See Also

### Accessing Message Content

var headers: [String : [String]]?

A dictionary that contains the message’s header values.

