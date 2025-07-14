

- Core Video
-  CVDisplayLinkStop(\_:) Deprecated

Function

# CVDisplayLinkStop(\_:)

Stops a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkStop(_ displayLink: CVDisplayLink) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link to be stopped.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

If the specified display link is already stopped, `CVDisplayLinkStop` returns an error.

In macOS 10.4 and later, the display link thread is automatically stopped if the user employs Fast User Switching. The display link is restarted when switching back to the original user.

## See Also

### Managing Display Links

func CVDisplayLinkStart(CVDisplayLink) -> CVReturn

Activates a display link.

Deprecated

