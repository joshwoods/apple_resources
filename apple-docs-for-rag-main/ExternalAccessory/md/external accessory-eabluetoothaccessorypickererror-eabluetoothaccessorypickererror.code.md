

- External Accessory
- EABluetoothAccessoryPickerError
-  EABluetoothAccessoryPickerError.Code 

Enumeration

# EABluetoothAccessoryPickerError.Code

The error codes that may be passed in an error object for the Bluetooth picker completion block.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case alreadyConnected

The specified accessory was already connected.

case resultNotFound

The specified accessory could not be found, perhaps because it was turned off prior to connection.

case resultCancelled

The user canceled the picker alert.

case resultFailed

Selecting an accessory failed for an unknown reason.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Presenting the Bluetooth Picker

func showBluetoothAccessoryPicker(withNameFilter: NSPredicate?, completion: EABluetoothAccessoryPickerCompletion?)

Displays an alert that allows the user to pair the device with a Bluetooth accessory.

typealias EABluetoothAccessoryPickerCompletion

The completion block for the Bluetooth picker.

struct EABluetoothAccessoryPickerError

Error codes returned by the Bluetooth accessory picker.

let EABluetoothAccessoryPickerErrorDomain: String

The domain for errors passed to a Bluetooth picker completion block.

