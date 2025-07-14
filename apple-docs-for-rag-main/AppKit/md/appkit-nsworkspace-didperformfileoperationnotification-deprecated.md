

- AppKit
- NSWorkspace
-  didPerformFileOperationNotification Deprecated

Type Property

# didPerformFileOperationNotification

Posted when a file operation has been performed in the receiving app.

macOS 10.0–10.11Deprecated

``` source
class let didPerformFileOperationNotification: NSNotification.Name
```

## Discussion

The notification object is the shared `NSWorkspace` instance. The `userInfo` dictionary contains a key `@"NSOperationNumber"` with a `NSNumber` object containing an integer indicating the type of file operation

