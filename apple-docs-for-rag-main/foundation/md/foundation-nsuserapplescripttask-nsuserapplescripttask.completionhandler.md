

- Foundation
- NSUserAppleScriptTask
-  NSUserAppleScriptTask.CompletionHandler 

Type Alias

# NSUserAppleScriptTask.CompletionHandler

Implement this block to retrieve the result of the AppleScript executed by execute(withAppleEvent:completionHandler:).

macOS 10.0+

``` source
typealias CompletionHandler = (NSAppleEventDescriptor?, (any Error)?) -> Void
```

