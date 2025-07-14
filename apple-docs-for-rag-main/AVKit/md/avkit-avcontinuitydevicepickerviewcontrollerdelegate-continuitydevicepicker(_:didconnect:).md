

- AVKit
- AVContinuityDevicePickerViewControllerDelegate
-  continuityDevicePicker(\_:didConnect:) 

Instance Method

# continuityDevicePicker(\_:didConnect:)

Informs the delegate when a person selects and connects a continuity device to the system with a continuity device picker.

tvOS 17.0+

``` source
optional func continuityDevicePicker(
    _ pickerViewController: AVContinuityDevicePickerViewController,
    didConnect device: AVContinuityDevice
)
```

## Parameters 

`pickerViewController`  

The continuity device picker that’s connecting `device` to the system.

`device`  

A continuity device that’s connecting to the system.

## See Also

### Responding to continuity device events

func continuityDevicePickerWillBeginPresenting(AVContinuityDevicePickerViewController)

Informs the delegate that a continuity device picker is about to present its UI so that a person can select and connect a continuity device.

func continuityDevicePickerDidCancel(AVContinuityDevicePickerViewController)

Informs the delegate when a person declines to select a continuity device by dismissing an app’s continuity device picker.

func continuityDevicePickerDidEndPresenting(AVContinuityDevicePickerViewController)

Informs the delegate that a continuity device picker is no longer presenting its UI to a person.

