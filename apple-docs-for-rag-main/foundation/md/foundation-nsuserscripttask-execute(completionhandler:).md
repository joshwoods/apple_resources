

- Foundation
- NSUserScriptTask
-  execute(completionHandler:) 

Instance Method

# execute(completionHandler:)

Executes the script with no input and ignoring any result.

macOS 10.8+

``` source
func execute(completionHandler handler: NSUserScriptTask.CompletionHandler? = nil)
```

``` source
func execute() async throws
```

## Parameters 

`handler`  

The completion handler Block that returns the result or an error. See NSUserScriptTask.CompletionHandler.

## Discussion

This method should be invoked no more than once for a given instance of the class.

If the script completed normally, the completion handler’s `error` parameter will be `nil`.

## See Also

### Related Documentation

init(url: URL) throws

Return a user script task instance given a URL for a script file.

