

- Core NFC
- CardSession
-  alertMessage 

Instance Property

# alertMessage

A message to show on the alert action sheet after card emulation starts.

iOS 17.4+iPadOS 17.4+

``` source
var alertMessage: String { get set }
```

## Discussion

Use this string to provide additional context about the NFC card emulation process. You can update this string in any thread context as long as the session is valid. Set this value prior to calling startEmulation() to display an appropriate message.

