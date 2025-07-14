

- Quartz
- IKDeviceBrowserView
-  delegate 

Instance Property

# delegate

Specifies the delegate object.

macOS 10.6+

``` source
@IBOutlet @MainActor
unowned(unsafe) var delegate: (any IKDeviceBrowserViewDelegate)! { get set }
```

## Discussion

The delegate object must conform to the IKDeviceBrowserViewDelegate protocol.

