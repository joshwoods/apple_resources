

- Objective-C Runtime
- NSObject
-  commitComposition(\_:) 

Instance Method

# commitComposition(\_:)

Informs the controller that the composition should be committed.

macOS

``` source
func commitComposition(_ sender: Any!)
```

## Parameters 

`sender`  

The client object requesting the input method to commit the composition.

## Discussion

If an input method implements this method, it is called when the client wants to end the composition session immediately. A typical response would be to call the `insertText` method of the client and then clean up any per-session buffers and variables. After receiving this message an input method should consider the given composition session finished.

