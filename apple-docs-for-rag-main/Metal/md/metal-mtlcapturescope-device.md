

- Metal
- MTLCaptureScope
-  device 

Instance Property

# device

The device object from which you created the capture scope.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## See Also

### Identifying the Capture Scope

var label: String?

A string that identifies the capture scope.

**Required**

var commandQueue: (any MTLCommandQueue)?

The command queue that this capture scope uses to limit which commands are recorded.

**Required**

