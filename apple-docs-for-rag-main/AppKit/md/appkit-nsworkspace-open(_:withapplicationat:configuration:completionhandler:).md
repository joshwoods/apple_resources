

- AppKit
- NSWorkspace
-  open(\_:withApplicationAt:configuration:completionHandler:) 

Instance Method

# open(\_:withApplicationAt:configuration:completionHandler:)

Opens one or more URLs asynchronously in the specified app using the provided options.

macOS 10.15+

``` source
func open(
    _ urls: [URL],
    withApplicationAt applicationURL: URL,
    configuration: NSWorkspace.OpenConfiguration,
    completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)? = nil
)
```

``` source
func open(
    _ urls: [URL],
    withApplicationAt applicationURL: URL,
    configuration: NSWorkspace.OpenConfiguration
) async throws -> NSRunningApplication
```

## Parameters 

`urls`  

The URL to open.

`applicationURL`  

A URL specifying the location of the app in the file system.

`configuration`  

The options that indicate how you want to open the URLs.

`completionHandler`  

The completion handler block to call asynchronously with the results. AppKit executes the completion handler on a concurrent queue. The handler block has no return value and takes the following parameters:

app  
On success, this parameter contains a reference to the app that opened the URLs. If the app didn’t open the URLs successfully, this parameter is `nil`.

error  
On failure, this parameter contains an NSError object indicating the reason for the failure. If the method opened the URLs successfully, this parameter is `nil`.

## Discussion

You may call this method safely from any thread of your app.

## See Also

### Opening URLs

func open(URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens a URL asynchronously using the provided options.

func open(URL) -> Bool

Opens the location at the specified URL.

