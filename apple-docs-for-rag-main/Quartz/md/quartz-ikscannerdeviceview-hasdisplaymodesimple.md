

- Quartz
- IKScannerDeviceView
-  hasDisplayModeSimple 

Instance Property

# hasDisplayModeSimple

The property that determines whether the scanner view uses the simple display mode.

macOS 10.6+

``` source
@MainActor
var hasDisplayModeSimple: Bool { get set }
```

## Discussion

If you create an `IKScannerDeviceView` object programmatically and want to use the simple display mode, do the following:

- Set this property to true.

- Set IKScannerDeviceViewDisplayMode.advanced to false.

- Set mode to IKScannerDeviceViewDisplayMode.simple.

The default value for this property is false.

## See Also

### Setting the Device View’s Display Mode

var mode: IKScannerDeviceViewDisplayMode

The display mode used by the device view.

var hasDisplayModeAdvanced: Bool

The property that determines whether the scanner view uses the advanced display mode.

