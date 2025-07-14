

- Safari Services
- SFSafariExtensionHandling
-  messageReceivedFromContainingApp(withName:userInfo:) 

Instance Method

# messageReceivedFromContainingApp(withName:userInfo:)

A method the system calls when the extension receives a message from the extension’s containing app.

macOS 10.12.4+

``` source
optional func messageReceivedFromContainingApp(
    withName messageName: String,
    userInfo: [String : Any]? = nil
)
```

## Parameters 

`messageName`  

A string that identifies the message.

`userInfo`  

Optional message content.

## See Also

### Related Documentation

class func dispatchMessage(withName: String, toExtensionWithIdentifier: String, userInfo: [String : Any]?, completionHandler: (((any Error)?) -> Void)?)

Sends a message to a Safari app extension, launching Safari if necessary.

### Receiving Messages in Your App Extension

func messageReceived(withName: String, from: SFSafariPage, userInfo: [String : Any]?)

A method the system calls when the extension receives a message from an injected script.

