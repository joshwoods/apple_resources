

- Metal
- MTLCaptureScope
-  label 

Instance Property

# label

A string that identifies the capture scope.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Setting this property on a capture scope makes it easier to discover specific capture scopes in Xcode. See `Label Your Capture Scope for Use in the Debug Bar`.

## See Also

### Identifying the Capture Scope

var device: any MTLDevice

The device object from which you created the capture scope.

**Required**

var commandQueue: (any MTLCommandQueue)?

The command queue that this capture scope uses to limit which commands are recorded.

**Required**

