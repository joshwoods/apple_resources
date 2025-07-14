

- Foundation
- NSUserAppleScriptTask
-  execute(withAppleEvent:completionHandler:) 

Instance Method

# execute(withAppleEvent:completionHandler:)

Execute the AppleScript script by sending it the specified Apple event.

macOS 10.8+

``` source
func execute(
    withAppleEvent event: NSAppleEventDescriptor?,
    completionHandler handler: NSUserAppleScriptTask.CompletionHandler? = nil
)
```

``` source
func execute(withAppleEvent event: NSAppleEventDescriptor?) async throws -> NSAppleEventDescriptor
```

## Parameters 

`event`  

The Apple event.

`handler`  

The completion handler Block that returns the result or an error. See NSUserAppleScriptTask.CompletionHandler.

## Discussion

Pass `nil` as `event` to execute the script’s default “run” handler.

This method should be invoked no more than once for a given instance of the class.

If the script completed normally, the completion handler’s `error` parameter will be `nil`.

## See Also

### Related Documentation

init(url: URL) throws

Return a user script task instance given a URL for a script file.

