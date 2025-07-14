

- AppKit
- NSWorkspace
-  openApplication(at:configuration:completionHandler:) 

Instance Method

# openApplication(at:configuration:completionHandler:)

Launches the app at the specified URL and asynchronously reports back on the app’s status.

macOS 10.15+

``` source
func openApplication(
    at applicationURL: URL,
    configuration: NSWorkspace.OpenConfiguration,
    completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)? = nil
)
```

``` source
func openApplication(
    at applicationURL: URL,
    configuration: NSWorkspace.OpenConfiguration
) async throws -> NSRunningApplication
```

## Parameters 

`applicationURL`  

A URL specifying the location of the app in the file system.

`configuration`  

The options that indicate how you want to launch the app.

`completionHandler`  

The completion handler block to call asynchronously with the results. AppKit executes the completion handler on a concurrent queue. The handler block has no return value and takes the following parameters:

app  
On success, this parameter contains a reference to the launched app. If the app wasn’t launched, this parameter is `nil`.

error  
On failure, this parameter contains an NSError object indicating the reason for the failure. If the app launched successfully, this parameter is `nil`.

## Discussion

## See Also

### Launching and Hiding Apps

func hideOtherApplications()

Hides all applications other than the sender.

