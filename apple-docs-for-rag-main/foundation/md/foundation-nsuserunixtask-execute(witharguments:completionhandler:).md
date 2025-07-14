

- Foundation
- NSUserUnixTask
-  execute(withArguments:completionHandler:) 

Instance Method

# execute(withArguments:completionHandler:)

Execute the unix script with the specified arguments.

macOS 10.8+

``` source
func execute(
    withArguments arguments: [String]?,
    completionHandler handler: NSUserUnixTask.CompletionHandler? = nil
)
```

``` source
func execute(withArguments arguments: [String]?) async throws
```

## Parameters 

`arguments`  

An array of `NSString` objects containing the script arguments. The arguments do not undergo shell expansion, so you do not need to do special quoting, and shell variables are not resolved.

`handler`  

The completion handler Block that returns the result. See NSUserUnixTask.CompletionHandler.

## Discussion

This method should be invoked no more than once for a given instance of the class.

If the script completed normally, the completion handler’s `error` parameter will be `nil`.

## See Also

### Related Documentation

var standardOutput: FileHandle?

The standard output stream.

var standardError: FileHandle?

The standard error stream.

init(url: URL) throws

Return a user script task instance given a URL for a script file.

var standardInput: FileHandle?

The standard input stream.

