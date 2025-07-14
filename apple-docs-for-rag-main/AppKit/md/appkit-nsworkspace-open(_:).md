

- AppKit
- NSWorkspace
-  open(\_:) 

Instance Method

# open(\_:)

Opens the location at the specified URL.

macOS

``` source
func open(_ url: URL) -> Bool
```

## Parameters 

`url`  

A URL specifying the location to open.

## Return Value

true if the location was successfully opened; otherwise, false.

## Discussion

You can call this method safely from any thread in macOS 10.6 and later.

## See Also

### Opening URLs

func open(URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens a URL asynchronously using the provided options.

func open([URL], withApplicationAt: URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens one or more URLs asynchronously in the specified app using the provided options.

