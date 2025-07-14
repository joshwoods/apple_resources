

- External Accessory
-  EABluetoothAccessoryPickerErrorDomain 

Global Variable

# EABluetoothAccessoryPickerErrorDomain

The domain for errors passed to a Bluetooth picker completion block.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
let EABluetoothAccessoryPickerErrorDomain: String
```

## See Also

### Presenting the Bluetooth Picker

func showBluetoothAccessoryPicker(withNameFilter: NSPredicate?, completion: EABluetoothAccessoryPickerCompletion?)

Displays an alert that allows the user to pair the device with a Bluetooth accessory.

typealias EABluetoothAccessoryPickerCompletion

The completion block for the Bluetooth picker.

struct EABluetoothAccessoryPickerError

Error codes returned by the Bluetooth accessory picker.

enum Code

The error codes that may be passed in an error object for the Bluetooth picker completion block.

