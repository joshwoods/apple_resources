

- Core Video
-  CVDisplayLinkStart(\_:) Deprecated

Function

# CVDisplayLinkStart(\_:)

Activates a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkStart(_ displayLink: CVDisplayLink) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link to be activated.

## Return Value

A Core Video result code. SeeCore Video Constants for possible values.

## Discussion

Calling this function starts the display link thread, which then periodically calls back to your application to request that you display frames. If the specified display link is already running, `CVDisplayLinkStart` returns an error.

## See Also

### Managing Display Links

func CVDisplayLinkStop(CVDisplayLink) -> CVReturn

Stops a display link.

Deprecated

