

- Foundation
- NSUserAutomatorTask
-  execute(withInput:completionHandler:) 

Instance Method

# execute(withInput:completionHandler:)

Execute the Automator workflow by providing it as securely coded input.

macOS 10.8+

``` source
func execute(
    withInput input: (any NSSecureCoding)?,
    completionHandler handler: NSUserAutomatorTask.CompletionHandler? = nil
)
```

``` source
func execute(withInput input: (any NSSecureCoding)?) async throws -> Any
```

## Parameters 

`input`  

The automator task.

`handler`  

The completion handler Block that returns the result or an error. See NSUserAutomatorTask.CompletionHandler.

## Discussion

The Automator workflow will execute using the variables property values.

This method should be invoked no more than once for a given instance of the class.

If the script completed normally, the completion handler’s `error` parameter will be `nil`.

## See Also

### Related Documentation

init(url: URL) throws

Return a user script task instance given a URL for a script file.

### Executing Automator Tasks

var variables: [String : Any]?

The variables required by the Automator workflow.

