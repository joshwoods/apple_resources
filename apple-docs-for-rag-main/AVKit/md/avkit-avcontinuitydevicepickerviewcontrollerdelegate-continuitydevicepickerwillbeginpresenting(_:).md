

- AVKit
- AVContinuityDevicePickerViewControllerDelegate
-  continuityDevicePickerWillBeginPresenting(\_:) 

Instance Method

# continuityDevicePickerWillBeginPresenting(\_:)

Informs the delegate that a continuity device picker is about to present its UI so that a person can select and connect a continuity device.

tvOS 17.0+

``` source
optional func continuityDevicePickerWillBeginPresenting(_ pickerViewController: AVContinuityDevicePickerViewController)
```

## Parameters 

`pickerViewController`  

The continuity device picker that’s informing the delegate.

## See Also

### Responding to continuity device events

func continuityDevicePickerDidCancel(AVContinuityDevicePickerViewController)

Informs the delegate when a person declines to select a continuity device by dismissing an app’s continuity device picker.

func continuityDevicePicker(AVContinuityDevicePickerViewController, didConnect: AVContinuityDevice)

Informs the delegate when a person selects and connects a continuity device to the system with a continuity device picker.

func continuityDevicePickerDidEndPresenting(AVContinuityDevicePickerViewController)

Informs the delegate that a continuity device picker is no longer presenting its UI to a person.

