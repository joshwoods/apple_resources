

- AppKit
- NSWorkspace
-  open(\_:configuration:completionHandler:) 

Instance Method

# open(\_:configuration:completionHandler:)

Opens a URL asynchronously using the provided options.

macOS 10.15+

``` source
func open(
    _ url: URL,
    configuration: NSWorkspace.OpenConfiguration,
    completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)? = nil
)
```

``` source
func open(
    _ url: URL,
    configuration: NSWorkspace.OpenConfiguration
) async throws -> NSRunningApplication
```

## Parameters 

`url`  

The URL to open.

`configuration`  

The options that indicate how you want to open the URL.

`completionHandler`  

The completion handler block to call asynchronously with the results. AppKit executes the completion handler on a concurrent queue. The handler block has no return value and takes the following parameters:

app  
On success, this parameter contains a reference to the app that opened the URL. If the app didn’t open the URL successfully, this parameter is `nil`.

error  
On failure, this parameter contains an NSError object indicating the reason for the failure. If the method opened the URL successfully, this parameter is `nil`.

## Discussion

You may call this method safely from any thread of your app.

## See Also

### Opening URLs

func open([URL], withApplicationAt: URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens one or more URLs asynchronously in the specified app using the provided options.

func open(URL) -> Bool

Opens the location at the specified URL.

