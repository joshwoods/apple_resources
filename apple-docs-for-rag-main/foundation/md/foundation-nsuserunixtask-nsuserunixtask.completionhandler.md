

- Foundation
- NSUserUnixTask
-  NSUserUnixTask.CompletionHandler 

Type Alias

# NSUserUnixTask.CompletionHandler

Implement this block to retrieve an error from the Unix scripted executed by execute(withArguments:completionHandler:).

macOS 10.0+

``` source
typealias CompletionHandler = ((any Error)?) -> Void
```

