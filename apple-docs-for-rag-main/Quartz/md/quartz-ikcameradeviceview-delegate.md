

- Quartz
- IKCameraDeviceView
-  delegate 

Instance Property

# delegate

The camera device view delegate.

macOS 10.6+

``` source
@IBOutlet @MainActor
unowned(unsafe) var delegate: (any IKCameraDeviceViewDelegate)! { get set }
```

## Discussion

The delegate must conform to the IKCameraDeviceViewDelegate protocol.

