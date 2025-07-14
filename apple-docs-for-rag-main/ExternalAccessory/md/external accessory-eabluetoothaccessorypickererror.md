

- External Accessory
-  EABluetoothAccessoryPickerError 

Structure

# EABluetoothAccessoryPickerError

Error codes returned by the Bluetooth accessory picker.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
struct EABluetoothAccessoryPickerError
```

## Topics

### Error Codes

static var alreadyConnected: EABluetoothAccessoryPickerError.Code

static var resultCancelled: EABluetoothAccessoryPickerError.Code

static var resultFailed: EABluetoothAccessoryPickerError.Code

static var resultNotFound: EABluetoothAccessoryPickerError.Code

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Presenting the Bluetooth Picker

func showBluetoothAccessoryPicker(withNameFilter: NSPredicate?, completion: EABluetoothAccessoryPickerCompletion?)

Displays an alert that allows the user to pair the device with a Bluetooth accessory.

typealias EABluetoothAccessoryPickerCompletion

The completion block for the Bluetooth picker.

enum Code

The error codes that may be passed in an error object for the Bluetooth picker completion block.

let EABluetoothAccessoryPickerErrorDomain: String

The domain for errors passed to a Bluetooth picker completion block.

