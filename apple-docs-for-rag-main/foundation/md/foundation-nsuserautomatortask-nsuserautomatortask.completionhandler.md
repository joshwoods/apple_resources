

- Foundation
- NSUserAutomatorTask
-  NSUserAutomatorTask.CompletionHandler 

Type Alias

# NSUserAutomatorTask.CompletionHandler

Implement this block to retrieve the output of the Automator workflow executed by execute(withInput:completionHandler:).

macOS 10.0+

``` source
typealias CompletionHandler = (Any?, (any Error)?) -> Void
```

