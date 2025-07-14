

- IOBluetooth UI
- IOBluetoothPairingController
-  addAllowedUUID(\_:) 

Instance Method

# addAllowedUUID(\_:)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

macOS 10.2+

``` source
@MainActor
func addAllowedUUID(_ allowedUUID: IOBluetoothSDPUUID!)
```

## Parameters 

`allowedUUID`  

UUID that a device may contain to be selected

## Discussion

The user’s device selection gets validated against the UUIDs passed to -addAllowedUUID: addAllowedUUIDArray:. Each call to those methods essentially adds a filter that the selected device gets validated with. If any of the filters match, the device is considered valid. If they all fail, the device is not valid and the user is presented with an error code that the device does not support the required services. The UUID passed to -addAllowedUUID: is the only UUID that must be present in the device’s SDP service records. Alternatively, all of the UUIDs in the UUID array passed to -addAllowedUUIDArray must be present.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

## See Also

### Instance Methods

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getResults() -> [Any]!

Returns an NSArray of the devices that were paired.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func runModal() -> Int32

Runs the pairing panel in a modal session to allow the user to select a Bluetooth device.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Sets the option bits that control the panel’s behavior.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

