

- AppKit
- NSApplication
- NSApplication.RequestUserAttentionType
-  NSApplication.RequestUserAttentionType.informationalRequest 

Case

# NSApplication.RequestUserAttentionType.informationalRequest

The user attention request is an informational request.

macOS

``` source
case informationalRequest
```

## Discussion

The dock icon will bounce for one second. The request, though, remains active until either the app becomes active or the request is canceled.

## See Also

### Constants

case criticalRequest

The user attention request is a critical request.

