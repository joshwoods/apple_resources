

- Foundation
- NSUserScriptTask
-  NSUserScriptTask.CompletionHandler 

Type Alias

# NSUserScriptTask.CompletionHandler

Implement this block to retrieve the error of the script executed by execute(completionHandler:).

macOS 10.0+

``` source
typealias CompletionHandler = ((any Error)?) -> Void
```

