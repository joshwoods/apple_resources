

- AppKit
- NSApplication
-  cancelUserAttentionRequest(\_:) 

Instance Method

# cancelUserAttentionRequest(\_:)

Cancels a previous user attention request.

macOS

``` source
@MainActor
func cancelUserAttentionRequest(_ request: Int)
```

## Parameters 

`request`  

The request identifier returned by the requestUserAttention(_:) method.

## Discussion

A request is also canceled automatically by user activation of the app.

## See Also

### Managing User Attention Requests

func requestUserAttention(NSApplication.RequestUserAttentionType) -> Int

Starts a user attention request.

enum RequestUserAttentionType

These constants specify the level of severity of a user attention request and are used by cancelUserAttentionRequest(_:) and requestUserAttention(_:).

func reply(toOpenOrPrint: NSApplication.DelegateReply)

Handles errors that might occur when the user attempts to open or print files.

enum DelegateReply

Constants that indicate whether a copy or print operation was successful, was canceled, or failed.

