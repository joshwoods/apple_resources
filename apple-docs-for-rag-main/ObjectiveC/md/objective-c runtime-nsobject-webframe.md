

- Objective-C Runtime
- NSObject
-  webFrame 

Instance Property

# webFrame

Returns the `WebFrame` that contains the plug-in.

macOS

``` source
var webFrame: WebFrame! { get }
```

## Return Value

The WebFrame that contains the plug-in.

## Discussion

Only implemented by containers that are based on the WebKit’s plug-in architecture.

## See Also

### Obtaining information about the container

var webPlugInContainerSelectionColor: NSColor!

Returns the plug-in selection color.

