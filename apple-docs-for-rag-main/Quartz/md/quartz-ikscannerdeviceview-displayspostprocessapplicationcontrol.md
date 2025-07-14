

- Quartz
- IKScannerDeviceView
-  displaysPostProcessApplicationControl 

Instance Property

# displaysPostProcessApplicationControl

Specifies whether the post processing application control is displayed.

macOS 10.6+

``` source
@MainActor
var displaysPostProcessApplicationControl: Bool { get set }
```

## Discussion

The post processing application is only relevant when the transfer mode is IKScannerDeviceViewTransferMode.fileBased.

## See Also

### Specifying a Post Processing Application

var postProcessApplication: URL!

The URL of the application to use for post processing of the scan.

