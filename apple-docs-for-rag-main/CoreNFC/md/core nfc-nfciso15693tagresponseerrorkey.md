

- Core NFC
-  NFCISO15693TagResponseErrorKey 

Global Variable

# NFCISO15693TagResponseErrorKey

A user information dictionary key indicating that a tag responded with a command error.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
let NFCISO15693TagResponseErrorKey: String
```

## Discussion

Check for the presence of this key in the userInfo dictionary of an NSError object to determine whether a tag responded with a command error. When a command error occurs, the code property contains an error code defined in the ISO15693-3 specification.

