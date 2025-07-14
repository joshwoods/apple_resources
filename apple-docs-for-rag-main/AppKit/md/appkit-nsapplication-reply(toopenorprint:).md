

- AppKit
- NSApplication
-  reply(toOpenOrPrint:) 

Instance Method

# reply(toOpenOrPrint:)

Handles errors that might occur when the user attempts to open or print files.

macOS

``` source
@MainActor
func reply(toOpenOrPrint reply: NSApplication.DelegateReply)
```

## Parameters 

`reply`  

The error that occurred. For a list of possible values, see NSApplication.DelegateReply.

## Discussion

Delegates should invoke this method if an error is encountered in the application(_:openFiles:) or application(_:printFiles:withSettings:showPrintPanels:) delegate methods.

## See Also

### Managing User Attention Requests

func requestUserAttention(NSApplication.RequestUserAttentionType) -> Int

Starts a user attention request.

enum RequestUserAttentionType

These constants specify the level of severity of a user attention request and are used by cancelUserAttentionRequest(_:) and requestUserAttention(_:).

func cancelUserAttentionRequest(Int)

Cancels a previous user attention request.

enum DelegateReply

Constants that indicate whether a copy or print operation was successful, was canceled, or failed.

