

- Quartz
- IKScannerDeviceView
-  postProcessApplication 

Instance Property

# postProcessApplication

The URL of the application to use for post processing of the scan.

macOS 10.6+

``` source
@MainActor
var postProcessApplication: URL! { get set }
```

## Discussion

The post processing application is only relevant when the transfer mode is IKScannerDeviceViewTransferMode.fileBased.

## See Also

### Specifying a Post Processing Application

var displaysPostProcessApplicationControl: Bool

Specifies whether the post processing application control is displayed.

