

- Quartz
- IKScannerDeviceView
-  delegate 

Instance Property

# delegate

The scanner device delegate

macOS 10.6+

``` source
@IBOutlet @MainActor
unowned(unsafe) var delegate: (any IKScannerDeviceViewDelegate)! { get set }
```

## Discussion

The delegate is sent notifications of errors as well as the completed scan content.

The delegate must conform to the IKScannerDeviceViewDelegate protocol.

