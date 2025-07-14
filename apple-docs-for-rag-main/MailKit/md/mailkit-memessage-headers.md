

- MailKit
- MEMessage
-  headers 

Instance Property

# headers

A dictionary that contains the message’s header values.

macOS 12.0+

``` source
var headers: [String : [String]]? { get }
```

## Discussion

If MailKit hasn’t downloaded the full message, this dictionary may only contain a subset of the message’s headers.

## See Also

### Accessing Message Content

var rawData: Data?

The raw RFC 2822 header and body content of the message.

