

- Safari Services
- SFSafariExtensionHandling
-  messageReceived(withName:from:userInfo:) 

Instance Method

# messageReceived(withName:from:userInfo:)

A method the system calls when the extension receives a message from an injected script.

macOS 10.12+

``` source
optional func messageReceived(
    withName messageName: String,
    from page: SFSafariPage,
    userInfo: [String : Any]? = nil
)
```

## Parameters 

`messageName`  

A string that identifies the message.

`page`  

The page that sent the message.

`userInfo`  

Optional message content. If specified, the dictionary’s value objects conform to the W3C standard for safe passing of structured data, such as Boolean objects, numeric values, strings, and arrays.

## Mentioned in 

Passing messages between Safari app extensions and injected scripts

## See Also

### Receiving Messages in Your App Extension

func messageReceivedFromContainingApp(withName: String, userInfo: [String : Any]?)

A method the system calls when the extension receives a message from the extension’s containing app.

